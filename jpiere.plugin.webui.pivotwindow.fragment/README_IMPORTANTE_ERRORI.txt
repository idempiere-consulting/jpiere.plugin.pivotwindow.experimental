In caso di errori maven per recupero jar di zk, principalmente zkpoi.jar e zkpoiex.jar, bisogna installarli manualmente nel repository locale .m2

Posizionarsi all'interno di questa cartella dove risiedono i jar e seguire i seguenti comandi:

1)  mvn install:install-file -DgroupId=org.zkoss.poi -DartifactId=zpoi -Dversion=3.9.7 -Dpackaging=jar -Dfile=zpoi-3.9.7.jar
2)  mvn install:install-file -DgroupId=org.zkoss.poi -DartifactId=zpoiex -Dversion=3.9.7 -Dpackaging=jar -Dfile=zpoiex-3.9.7.jar

Una volta fatto ciò, ri-aggiornare il progetto maven e ricompilare.
