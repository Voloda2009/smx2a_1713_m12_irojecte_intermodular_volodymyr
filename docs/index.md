# Sobre nuestro sitio web!

## Restaurante de proximidad La Taula del Barri 
<img src="Img\2026-10-08_190848747.png" width="20%">

## 1.Concepto y descripción del negocio

#### Descripción de la actividad: Cocina casera, productos locales y ambiente familiar.

#### Problema que resuelve la aplicación: Pasar de una gestión caótica de reservas (llamadas, mensajes y notas dispersas) a un sistema automatizado de reservas a través del navegador.
<br>

## 2.Información sobre horarios y condiciones
<br>

#### Días de apertura: De lunes a sábado (domingo cerrado).
<br>

#### Horarios laborales:
##### De 13:00 a 15:00
##### De 20:00 a 22:00
<br>

#### Franjas horarias disponibles:
##### 13:00, 14:00, 20:00 y 21:00 (duración de cada reserva: 1 hora).
<br>

#### Capacidad: 
##### Capacidad: Hasta 12 personas por reserva.
<br>

#### Zona horaria: 
##### Hora local de Barcelona.
<br>

## 3.Secciones principales de la web
<br>

#### Inicio (Inici): Presentación del restaurante, estilo visual y botón directo «Hacer reserva».
<br>

#### Formulario de reserva (Reserva): Campos para los datos del cliente (nombre, teléfono, fecha y hora).
<br>

#### Horarios y contacto (Horari / On som): Días y horas de apertura, días cerrados y dirección física.
<br>

#### Chat de IA (Xat IA): Asistente inteligente para consultar disponibilidad y reservar mediante conversación.
<br>

#### Gestión / Privada (Accés personal): Panel exclusivo para el personal (con acceso protegido) para ver, crear, editar o cancelar reservas.
<br>

## 4.Restricciones técnicas y reglas de validación
<br>

#### La fecha no puede ser anterior a la fecha actual.
#### El restaurante debe estar abierto ese día.
#### La hora debe corresponder al horario laboral establecido.
#### La franja horaria debe estar libre (el sistema rechaza duplicados y evita solicitudes simultáneas para la misma hora).
<br>

## 5.Elementos visuales y técnicos de la vitrina
<br>

### Logotipo del restaurante
<img src="Img\Logo.jpg" width="80%">
<br>

### Capturas de pantalla reales (o maquetas)
<img src="Img\Web.jpg" width="100%">



## Lists

- Unordered list item
- Another item with **strong** text

1. Ordered step one
2. Ordered step two


## Code blocks

```python
def greet(name: str) -> str:
    return f"Hello, {name}"
```

```javascript
const users = [{ name: "Alice" }, { name: "Bob" }];
console.log(users.map((u) => u.name).join(", "));
```

```bash
curl -s https://www.devtoolsdaily.com/sitemap.xml | head -n 5
```

## Table

| Feature | Status | Notes |
| --- | :---: | --- |
| GFM Tables | Yes | Uses `remark-gfm` |
| Syntax Highlighting | Yes | Multiple languages |
| Inline Code | Yes | Styled with monospace |
