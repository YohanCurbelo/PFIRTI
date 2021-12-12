PFIRTI (Pipelined FIR Filter Type I)

Description: 
    1. Customazible, optimized and pipelined FIR Filter Type I.
    2. The order of the filter has to be even (odd number of coefficients) 
    and its coefficients symmetric.
    3. Customizable: The widths of input, output, and internal signals are 
    configurable, making natual growth and truncation of data possible. 
    4. Optimized: As filter coefficients are symmetric, only half of values 
    that are symmetric to the middle address of the shift register are summed.


Descripcion:
    1. Filtro FIR tipo I personalizable, optimizado y segmentado.
    2. El orden del filtro tiene que ser par (cantidad impar de coeficientes)
    y sus coeficientes simetricos.
    3. Personalizable: El ancho de la senyal de entrada, salida, e internas son 
    configurables, haciendo posible el truncado y el crecimiento natural de los 
    datos internos.
    4. Optimizado: Como el filtro es simetrico solo se realiza una suma de los 
    valores que son simetricos respecto a la direccion central del registro de 
    desplazamiento.



             _______________________________________________________________________________
reset    ____|
                  __________________________
i_enable ________|                          |______ ...
                 _______________________________
i_data   ________| data 1 | data 2 | data 3 |       ...
                                                                   __________________________
o_enable _____________________________________________ ... _______|                          |______
                                                                  ___________________________
o_data   _________________________________________________________| data 1 | data 2 | data 3 |______