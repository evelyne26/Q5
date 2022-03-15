# Q5
#include <stdio.h>

#include <stdlib.h>



Int main()

{



    FILE *fp1 = fopen (« projet1.fichier_source », « rb ») ;

    Int bytes ;

    Unsigned char buf[1024] ;

       If (fp1 == NULL) {

        Printf (« Impossible de lire le fichier et la copies a echoue \n », projet1.fichier_source) ;

        Return 0 ;

    }



    MD5_Init (&FILE) ;

    While ((bytes = fread (buf, 1, 1024, inFile)) != 0)

        MD5_Update (&FILE, buf, bytes) ;

    MD5_Final (c,&FILE) ;

    For(i = 0 ; i < MD5_DIGEST_LENGTH ; i++) printf(« %02x », c[i]) ;

    Printf («  %s\n », filename) ;

    Fclose (File) ;

    Return 0 ;

}
