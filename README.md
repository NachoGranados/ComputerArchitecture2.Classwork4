Curso: Arquitectura de Computadores II
Asunto: Instrucciones para ejecutar los ejercicios prácticos del Taller 4
Ambiente de trabajo: Linux en placa Jetson Nano Developer Kit

Nota:
- Se debe verificar la versión de "CUDA" con el siguiente comando:
```bash
$ nvcc --version
```
    
- En caso de que no se encuentre se debe verificar el archivo ∼/.bashrc contenga las siguientes líneas:
```bash
export PATH=/usr/local/cuda/bin${PATH:+:${PATH}}
export LD_LIBRARY_PATH=/usr/local/cuda/lib64${LD_LIBRARY_PATH (continua)
:+:${LD_LIBRARY_PATH}}
```

- Verificar nuevamente la versión para asegurarse que se hicieron los pasos correctamente.

1. Compilación de los ejercicios prácticos.

1.1. Compilación del primer ejercicio práctico. Dicha compilación se logra ejecutando el siguiente comando:
```bash
$ nvcc -o mult_mat.cu mult_mat
```

1.2. Compilación del segundo ejercicio práctico. Dicha compilación se logra ejecutando el siguiente comando:
```bash
$ nvcc -o saxpy.cu saxpy
```

2. Ejecución de los ejercicios prácticos.

2.1 Ejecución del primer ejercicio práctico. Dicha ejecución se logra ejecutando el siguiente comando:
```bash
$ ./mult_mat
```

2.1 Ejecución del segundo ejercicio práctico. Dicha ejecución se logra ejecutando el siguiente comando:
```bash
$ ./saxpy
```
