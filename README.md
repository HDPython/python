def short(lis):

   '''
   Juan Villate Isaza 06/04/2014
   Obj: por medio de parametro de una lista ordenar de menor a mayor la lista dada, con el numero de la mitad.
   pre: lista de enteros
   pos: retornar la lista ordenada.
   '''
   #ir pniendo los numeros de la lista hasta llegar a la mitad
   for i in range(len(lis)):
      #guardar el numero para despues compararlo
      num= lis[i]
      #Guardar la posicion anterior para 
      a = i-1
      
      #ir comparando con la lista y posicionandolo (luego de llegar a la interseccion de la lista).
      while (a >= 0 and lis[a] > num):
         #ir intercalando numeros para llegar al orden
         lis[a+1] = lis[a]
         a=a-1
         #pegar num a la lista
         lis[a+1]=num
         
   #imprime la lista ordenada
   print("finalmente:", lis)
      
