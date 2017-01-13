# Usenet - Verify-Signature-newzNZB
New field on newz[NZB] uploads "Verify-Signature-newzNZB"

newzNZB(1)                 Verify-Signature-newzNZB                     newzNZB(1)

NAME

    newzNZB: Verify-Signature.


TL;DR

    ~$ Go to our special verify tool site ( verify.newznzb.info ) and if the signature 
       is OURS the result will be:
	   
        ******************************************************************************	
		
	root% cmd:verify.newznzb.info --verify newzNZB.sig 
        echo: Signature made YEAR-MONTH-DAY HOUR:MINUTE:SECOND using TMP key ID ----
        echo: Good signature from "nEwZ[NZB]"

        Signature:
        [THERE WILL BE TEXTAREA WITH DECODED SIGNATURE]

	******************************************************************************
		
WHERE TO GET OUR SIGNATURE

     ~# If you are able to browse thru usenet, just find our posts and view all
	the headers of our messages.
        There you can find "Verify-Signature-newzNZB:" field, you need to copy whole
	signature so -
		
 ('-----BEGIN newzNZB SIGNATURE-----', 'SIGNATURE_STUFF', '<MSG_ID@PRiVATE>', '-----END newzNZB SIGNATURE-----')
 
WHY

     ~? On the usenet you are able to use any name you like, if someone decide become the
	same named uploader like we are, there is NO way to stop him/her. There we get to the 
	point what we can do about it? What if someone start posting FAKE/MALWARE/VIRUS
	posts. So we simply implement our own idea of Verify-Signature-newzNZB. We think we are
	the first in usenet uploaders who do it this way :)

CHANGELOG
    2017-JAN-13
        You can also verify now OUR signature thru your terminal (ssh and curl cmd) 
	via our api - check EXAMPLE_CURL file
    2017-JAN-12
        Idea, so we added it to our uploader software


TODO
    * (?)
