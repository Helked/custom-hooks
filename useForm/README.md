# useForm

Creamos una constante que recibirá del useForm los valores y funciones para manejar el formulario y establecemos el valor inicial del formulario

```
const [ values, handleInputChange, reset ] = useForm( initialState );
```

Cuando creemos un input, es **necesario** ponerle un **name** que **debe ser el mismo** que la variable que va a tener su valor

```
<input 
    type = "text"
    value = { nombreCampo }
    name = { nombreCampo }
    onChange = { handleInputChange }
/>
```

## values
Objeto que contiene el valor de cada uno de los elementos del formulario. Podemos desestructurarlo para obtener los valores:
```
const { nombreCampo } = values;
```


## handleInputChange 
Función que hay que añadir al *onChange* del input

## reset 
Función que tendríamos que llamar si queremos resetear el formulario