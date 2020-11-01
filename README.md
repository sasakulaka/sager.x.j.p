      PROGRAM TEXT11
	  REAL X0,X1,N
	  READ(*,*) X0
	  N=1
10    X1=1.+1./X0**2
      CONTINUE
	  IF(ABS(X1-X0)>7.5E-4)THEN
	  X0=X1
	  N=N+1
      GOTO 10
	  ENDIF
      WRITE(*,*)'X1=',X1,'N=',N
	  END
