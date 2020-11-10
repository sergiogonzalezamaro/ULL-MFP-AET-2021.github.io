![ULL Logo](https://www.ull.es/portal/noticias/wp-content/uploads/sites/13/2018/04/ull-nuevo-logo.jpg)

# Curriculum Vitae
## Datos generales
* **Nombre** {{site.data.cv.Nombre}}
* [Usuario ULL](https://campusdoctoradoyposgrado.ull.es/user/profile.php?id=34035)

## Educación
* Grado Universitario: {{site.data.cv.Grado_Universitario}}
* Idiomas: {{site.data.cv.Idiomas}}

### Cursos
{% for a in site.data.cv.Cursos %}
* {{ Cursos }}
{%- endfor %}

## Experiencia Laboral
* Puesto: {{site.data.cv.Puesto}}

## Cita favorita
Palabras de Yoda de Star Wars
> Que la fuerza te acompañe

## Código 
``` C++
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
<!-- if site.Programa = "Programa" -->
<!-- if site.Programa = "Nivel de conocimiento" -->
|Programa|Nivel de conocimiento|
|--------|--------|
|{{ site.Programa[0] }}|{{ site.Nivel de conocimiento[0] }}|
|{{ site.Programa[1] }}|{{ site.Nivel de conocimiento[1] }}|
|{{ site.Programa[2] }}|{{ site.Nivel de conocimiento[2] }}|

## Evaluación
- [ ] Todo ok? :call_me_hand:

## Experiencia Master
[Opinion Master](https://github.com/ULL-MFP-AET-2021/p02-t0-aprender-markdown-sergiogonzalezamaro/blob/main/master.md)
