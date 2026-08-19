# Red-Empresarial-Cisco
Hice una pequeña red empresarial donde tengo el router, trunks, switch y 4 PC cada una con distinto objetivo (admin, ventas, soporte y guest"
me dieron problemas de configuracion de trunks, dhcp, vlans y ping
resolvi haciendo router-on-a-stick con 4 subinterfaces dot1Q. dhcp funcionando por cada vlan (10,20,30,40). trunk en el puerto fisico correcto (Fa0/1). puertos de acceso bien asignados y ruteo inter-VLAN al 100%
Problema inicial: PCs no pingueaban entre vlans distintas
metodologia de diagnostico: fui capa por capa (fisica > enlace > red) usando "show mac address-table , show cdp neighbors, show vlan brief, show interfaces trunk.
errores encontrados y solucion: subinterfaz cruzada, STP sin portfast, trunk en puerto equivocado y vlan mal asignada
la configuracion final fue con el "show running.config" completo del router y switch (todavia no se como exportar los logs asique cuando aprenda subire con mas profesionalidad los archivos, logs y topologia)
