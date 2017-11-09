Feature D
=========

.. code-block:: fortran

   !   computation of pressure at half levels.
   CALL GPPRE(NPROMA,IST,IEND,NFLEVG,YRVAB%VAH,YRVAB%VBH,ZPRESH,ZPRESF)
   
   !   computation of auxiliary arrays for the hydrostatic.
   CALL GPXYB(NPROMA,IST,IEND,NFLEVG,YRVAB%VDELB,YRVAB%VC &
         &,ZPRESH,ZDELP0,ZRDELP0,ZLNPR0,ZALPH0,ZDUM,ZDUM,ZDUM)
   
   !   computation of r, cp and kappa.
   CALL GPRCP(NPROMA,IST,IEND,NFLEVG,QT0,ST0,WT0,ZDUM,ZDUM,ZDUM,ZCP0,ZR0,ZKAP)


