Enlace de descarga ROSBAG: https://drive.google.com/drive/folders/1NPpRjNa35FJ_zFsqB31bmQMJqmWvKQCR?hl=es-419

GRAFICAS
-
-- Aceleracion vs tiempo

![grafica_aceleracion](https://github.com/user-attachments/assets/2ad7e492-45a3-48f6-9e12-df995a25c3bb)

Esta gráfica muestra cómo varía la aceleración del robot a lo largo del tiempo en los ejes X, Y y Z. La aceleración en Z se mantiene cerca de 9.8 m/s², indicando que el IMU detecta correctamente la gravedad cuando el robot está en reposo o con movimiento vertical mínimo. En cambio, las aceleraciones en X y Y presentan oscilaciones y picos, especialmente entre los segundos 500 y 520, lo que sugiere movimientos rápidos o cambios de dirección cuandp el robot se desplazaba.

-- Posicion vs tiempo

![grafica_posicion_ruedas](https://github.com/user-attachments/assets/9e3cdbe5-4d29-4d31-90e8-1ab55982f279)

Esta gráfica muestra la posición angular de cada rueda del robot a lo largo del tiempo, indicando cuánto han girado desde el inicio. Al principio, las ruedas permanecen en reposo, y luego todas siguen trayectorias casi idénticas con incrementos escalonados, debido a los movimientos controlados en tramos. El hecho de que todas las ruedas muestren un patrón similar indica que se movieron de forma sincronizada. Cuando vemos que ciertas ruedas difieren un poco entre si es debido a los 
ultimos giros de orientacion.

-- Gasto vs tiempo

![grafica_esfuerzo_total](https://github.com/user-attachments/assets/a5d9a137-9031-467b-91b8-4c4142b6dad8)

La gráfica representa la suma del esfuerzo (torque) aplicado por todos los actuadores (joints) del robot en cada instante de tiempo. Se observan periodos de esfuerzo nulo cuando el robot está detenido, y picos positivos y negativos cuando está en movimiento o realiza maniobras exigentes. Los valores extremos, como los picos de ±200 Nm, indican momentos de mayor demanda de fuerza, como aceleraciones bruscas o frenadas, coincidiendo con los periodos de alta aceleración detectados por el IMU.
