## Numbers Project

#### Structure (HTML)

- section
  - article
    - span.number data-value="value" (0)
    - p (text)

#### Logic (JS)

- select all span's with .number
- iterate over and log each span
- create updateCount function
- accept el as argument
- invoke and pass each span el in iteration

```js
const updateCount = (el) => {
  const value = parseInt(el.dataset.value);
  const increment = Math.ceil(value / 1000);
  let initialValue = 0;
};
```

```js
const updateCount = (el) => {
  const value = parseInt(el.dataset.value);
  const increment = Math.ceil(value / 1000);
  let initialValue = 0;

  const increaseCount = setInterval(() => {
    initialValue += increment;

    if (initialValue > value) {
      el.textContent = `${value}+`;
      clearInterval(increaseCount);
      return;
    }
    el.textContent = `${initialValue}+`;
  }, 1);
};
```

## Contribuciones

Si deseas contribuir al proyecto, por favor envía un pull request o abre un issue para discutir los cambios que te gustaría implementar.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo `LICENSE` para obtener más detalles.

## Contacto

Si tienes alguna consulta, puedes contactar a [Martin Juncos](mailto:prof.mcjuncos@gmail.com).

                    ©Prof Martin Juncos
