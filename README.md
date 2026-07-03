<h2>🛒 Descripción general:</h2>
<br>
En este notebook se realiza un análisis de canasta de mercado mediante <b>Reglas de asociación</b> en dos sets de datos para comparar los resultados.<br><br>
• Las reglas de asociación son un método de minería de datos que consiste en identificar relaciones entre variables, útil en segmentación de clientes y análisis de cesta de compras: <br><br>
              <b>'Si un cliente compra A, es probable que también compre B' (antecedente -> consecuente).</b><br><br> 
• El objetivo es conocer las preferencias y hábitos de compra.<br>
• La información puede ser útil para optimizar promociones y distribución de inventarios.
<br><br>
El algoritmo <b>Apriori</b> es de los más utilizados en la minería de reglas de asociación. Identifica elementos que aparecen juntos con frecuencia para generar las reglas de asociación. En la poda (pruning) se eliminan conjuntos que no alcanzan un umbral mínimo de soporte, entre otros factores.<br>

<b> 
<h2>⚙️Tecnologías: </h2>
<br>
    • Python 3.10+<br>
    • Jupyter Notebook<br>
    • Pandas<br>
    • Itertools<br>
    • TransactionEncoder<br>
    • apriori<br>
    • association_rules<br>
<br>

<h2>🖇️ Fuentes: </h2><br>
https://www.kaggle.com/datasets/mysarahmadbhat/pizza-place-sales?select=pizzas.csv <br>
https://www.kaggle.com/datasets/rukenmissonnier/real-market-data

<br>
<br>

<h2>🧩 Variables:</h2
<br> • (Set de datos Pizzería): order_id	date,	time,	order_details_id,	pizza_id,	quantity,	pizza_type_id,	size,	price	name,	category,	ingredients.<br>
     • (Datos para Reglas de asociación de Mercado): Matriz binaria.
<br>
<br>
<br>
<h2>📊 Actividades: </h2>
<br>
    • Creación de listas por pares de elementos.<br>
    • Algoritmo Apriori y poda de conjuntos por distintos parámetros (Soporte, confianza, elevación, entre otros).<br>
    • Generación de reglas de asociación en dos sets de datos.<br>
    • Comparación de resultados.<br>
<br>
<br>
<h2>⭐ Conclusiones: </h2>
<br> 
    • En el primer ejemplo (Pizzería), las reglas de asociación generadas no tienen fuerza suficiente para ser útiles en insights de negocio:<br>
       • Existe una confianza del 5%.<br>
       • Independencia y asociación negativa entre antecedente -> consecuente.<br><br>
    • En el segundo ejemplo (Mercado), las reglas generadas sí tienen fuerza suficiente para ser útiles en insights de negocio: <br>
       • Confianza de 70%.<br>
       • Dependencia y asociación positiva entre antecedente -> consecuente.
