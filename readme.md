---
permalink: index.html
---
<img src="https://www.ull.es/portal/noticias/wp-content/uploads/sites/13/2018/04/ull-nuevo-logo.jpg" width="20%">

# Curriculum Vitae
## Datos generales
* **Nombre** {{site.data.cv.Nombre}}
* [Usuario ULL](https://campusdoctoradoyposgrado.ull.es/user/profile.php?id=34035)

## Educación
* Grado Universitario: {{site.data.cv.Grado_Universitario}}
* Idiomas: {{site.data.cv.Idiomas}}

### Cursos
{%- for a in site.data.cv.Cursos %}
* {{ a }}
{%- endfor %}

## Experiencia Laboral
* Puesto: {{site.data.cv.Puesto}}

## Cita favorita
Palabras de Yoda de Star Wars
> Que la fuerza te acompañe

## Código 
```cpp
void setup()
{
  pinMode(A1, INPUT);
  pinMode(13, OUTPUT);
  pinMode(11, OUTPUT);
}

void loop()
{
  if (analogRead(A1) > 500) {
    digitalWrite(13, HIGH);
    digitalWrite(11, HIGH);
    delay(1000); // Wait for 1000 millisecond(s)
    digitalWrite(11, LOW);
    digitalWrite(13, LOW);
    delay(1000); // Wait for 1000 millisecond(s)
  }
}
```
## Programas

|Programa|Nivel de conocimiento|
{%- for tabla in site.data.cv.Programas %}
|--------|--------|
|{{- tabla.Programa }}|{{ tabla.Nivel }}|
{%- endfor %}

## Evaluación
- [ ] Todo ok? :call_me_hand:

## Experiencia Master
[Opinion Master]({{site.baseurl}}/master)
