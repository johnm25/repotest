DISPLAY CHLAUTH('DEV.APP.SVRCONN') MATCH(RUNCHECK) ALL ADDRESS('192.168.99.1')  CLNTUSER('jkh')

andy til adgang


DISPLAY CHLAUTH(DEV.APP.SVRCONN) MATCH(RUNCHECK) ADDRESS(*) CLNTUSER(jkh)
		
Change MQ so no userid is needed		
ALTER QMGR CHLAUTH(DISABLED) CONNAUTH(' ')
REFRESH SECURITY TYPE(CONNAUTH)
ALTER CHANNEL('SYSTEM.DEF.SVRCONN) CHLTYPE(SVRCONN) MCAUSER('jkh')


sdf

Dev branch
