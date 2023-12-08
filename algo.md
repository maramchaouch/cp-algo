/**/
ALGORITHM cp
VAR/* the sentences*/
    ch:STRING;
    /*the counters*/
    i,j,nbv,nbw,longch:INTEGER;
    const voy:='aeyiuoAEYUIO';

    
BEGIN
/*parcour du chaine*/
    write('donner ch');
    read(ch);
    nbv=0;
    nbw=1;
    FOR i FROM 0 TO long(ch) STEP 1 DO;
        FOR j FROM 0 TO long(voy) STEP 1  DO
            IF (ch[i]=voy[j]) THEN
                nbv=nbv+1;
            END_IF
        END_FOR
        IF (ch[i]=' ') THEN;
            nbw=nbw+1
        END_IF
    END_FOR
    write(nbv,nbw,longch);
    
END
go my code.