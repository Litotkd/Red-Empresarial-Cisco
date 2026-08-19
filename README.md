# Red-Empresarial-Cisco
Hice una pequeña red empresarial donde tengo el router, trunks, switch y 4 PC cada una con distinto objetivo (admin, ventas, soporte y guest"
me dieron problemas de configuracion de trunks, dhcp, vlans y ping
resolvi haciendo router-on-a-stick con 4 subinterfaces dot1Q. dhcp funcionando por cada vlan (10,20,30,40). trunk en el puerto fisico correcto (Fa0/1). puerdos de acceso bien asignados y ruteo inter-VLAN al 100%
