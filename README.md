# Practica4APSI

  tipo: post  ruta: /cars/create  parametros: Un body{"tag"(matricula):string, "brand"(marca del coche):string, "model"(modelo del coche):string, "price"(precio del coche):number}
  
  tipo: post  ruta: /dealer/create  parametros: Un body{"name"(nombre del concesionario):string,"allowance"(permiso de venta):boolean}
  
  tipo: post  ruta: /client/create  parametros: Un body{"dni":string[9], "name"(nombre del cliente):string, "walletSize"(capital disponible del cliente):number}
  
  tipo: put  ruta: /dealer/addCar/:dealerName/:carTag  parametros: dealerName: Nombre del concesionario a modificar, carTag: matricula del cohe que se va a añadir
  
  tipo: get  ruta: /dealer/getAll/:dealerName  parametros: dealerName: Nombre del concesionario del que se mostraran todos los coches
  
  tipo: put  ruta: /dealer/sellCar/:dealerName/:clientDni/:carTag  parametros: dealerName: Nombre del concesionario que vendera el coche, carTag: Matricula del coche que se vende,
  clientDni: DNI del cliente que compra el coche
  
  tipo: get  ruta: /client/getAll/:dni  parametros: dni: El dni delcliente que quieres mostrar todos sus coches
  
  tipo: put  ruta: /dealer/deleteCar/:dealerName/:carTag  parametros: dealerName: El nombre del concesionario del que quieres borrar un coche, carTag: La matricula del coche a borrar
  
  tipo: put  ruta: /client/deleteCar/:dealerName/:carTag  parametros: dealerName: El nombre del cliente del que quieres borrar un coche, carTag: La matricula del coche a borrar
  
  tipo: put  ruta: /client/clientToClient/:client1/:client2/:carTag  parametros: client1: cliente que vende coche, client2: cliente que compra coche,
  carTag: Matricula del coche que se vende
  
  tipo: put  ruta: /client/addMoney/:client/:amount  parametros: client al que se le quiere añadir dinero, amount: cantidad de dinero que se añade
  
  tipo: put  ruta: /dealer/chengeAllowance/:dealerName  parametros: dealerName: Nombre del concesionario al que se le cambia el permiso de venta
  
  EXTRAS
  
  tipo: get  ruta: /showAllClients  parametros: Ninguno Muestra todos los clientes
  
  tipo: get  ruta: /showAllCars  parametros: Ninguno Muestra todos los coches
  
  tipo: get  ruta: /showAllDealers  parametros: Ninguno Muestra todos los concesionarios
  
