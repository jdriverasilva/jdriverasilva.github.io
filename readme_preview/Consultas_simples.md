# Consultas Simples #

## consultas Básicas ## 

**1. Selección de países en el continente 'Asia'**

**Álgebra relacional**:

$$
\sigma_{\text{Continent} = 'Asia'}(\text{Country})
$$

**SQL equivalente**:

```sql
SELECT * FROM country WHERE Continent = 'asia';
```
<div align="center">
<img src="./documentos/Universidad/Base de Datos/pantallazos simpleQueries.md/pregunta1.1.png" width=90%>
</div>

**2. Contar el número total de ciudades**

**Álgebra relacional**:

$$
\text{COUNT}(\text{City})
$$

**SQL equivalente**:  
```sql

```

**3. Listar todos los idiomas únicos en la tabla CountryLanguage**

**Álgebra relacional**:  

$$
\pi_{\text{Language}}(\text{CountryLanguage})
$$

**SQL equivalente**:  
```sql

```

**4. Selección de países con población mayor a 100 millones**

**Álgebra relacional**:  

$$
\sigma_{\text{Population} > 100000000}(\text{Country})
$$

**SQL equivalente**:  
```sql

```

**5. Listar nombres de países y continentes ordenados alfabéticamente por nombre de país**

**Álgebra relacional**:  

$$
\pi_{\text{Name}, \text{Continent}}(\text{Country}) \text{ ORDER BY Name}
$$

**SQL equivalente**:  
```sql

```

**6. Obtener la ciudad con mayor población**

**Álgebra relacional**:  

$$
\text{MAX}(\pi_{\text{Population}}(\text{City}))
$$

**SQL equivalente**:  
```sql

```

**7. Selección de países que tienen 'Republic' en su nombre**

**Álgebra relacional**:  

$$
\sigma_{\text{Name LIKE '%Republic%'}}(\text{Country})
$$

**SQL equivalente**:  
```sql

```

**8. Listar los 5 países más poblados**

**Álgebra relacional**:  

$$
\pi_{\text{Name, Population}}(\text{Country}) \text{ ORDER BY Population DESC LIMIT 5}
$$

**SQL equivalente**:  
```sql

```

**9. Calcular la población promedio de los países en el continente 'Europe'**

**Álgebra relacional**:  

$$
\text{AVG}(\pi_{\text{Population}}(\sigma_{\text{Continent} = 'Europe'}(\text{Country})))
$$

**SQL equivalente**:  
```sql

```

**10. Selección de idiomas con más del 10% de la población mundial que los habla**

**Álgebra relacional**:  

$$
\sigma_{\text{Percentage} > 10}(\text{CountryLanguage})
$$

**SQL equivalente**:  
```sql

```
