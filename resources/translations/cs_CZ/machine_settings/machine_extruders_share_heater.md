Extrudéry sdílí ohřev
====
Tímto nastavením můžete označit, že všechny trysky v této tiskárně sdílí jeden ohřev. Nebudou se zahřívat a ochlazovat vaše trysky jednotlivě, když se některé trysky znovu aktivují a stanou se neaktivní, ale pouze se udržují v teple.

Nejčastěji je to nutné pro směšovací trysky, kde se do stejné trysky přivádí více vláken. Tato tryska má pouze jeden ohřev, který zahřívá kterékoli vlákno uvnitř trysky. Pokud by Cura ovládala zahřívání pro každé vlákno zvlášť, pokusila by se současně udržet trysku horkou pro aktivní vlákno, zatímco by ji ochlazovala na [pohotovostní teplotu](../material/material_standby_temperature.md) pro ostatní vlákna. To je nemožné a mělo by to za následek buď zahřátí pouze na prvního vlákna, nebo trvalý tisk při pohotovostní teplotě, pokud firmware pouze aplikuje příkazy pro ohřev na jednu trysku bez ohledu na to, na který nástroj jsou zaměřeny. To, že extrudéry sdílejí ohřívač, naznačuje aplikaci Cura, aby tomuto problému zabránila. Cura již nebude pouštět trysku do pohotovostní teploty a už nebude používat žádný příkaz k ohřevu pro žádný konkrétní extrudér.

Cura nemusí nutně předpokládat, že pokud extrudéry sdílejí ohřev, sdílejí také trysku. Pokud ano, musí být relativní polohy trysek 0 a nejpravděpodobnější je, že musí být k dispozici určitá počáteční sekvence extrudéru, aby se při přepnutí propláchl předchozí materiál.

*Protože se jedná o nastavení stroje, nebude obvykle uvedeno v normálním seznamu nastavení. Zaškrtávací políčko pro toto nastavení je však v dialogu nastavení tiskárny, které lze nalézt v seznamu přidaných tiskáren v dialogu předvoleb.*