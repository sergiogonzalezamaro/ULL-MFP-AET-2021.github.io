![ULL Logo](https://www.ull.es/portal/noticias/wp-content/uploads/sites/13/2018/04/ull-nuevo-logo.jpg)

# Curriculum Vitae
## Datos generales
* **Nombre** Sergio González Amaro
* Usuario [ULL] (https://campusdoctoradoyposgrado.ull.es/user/profile.php?id=34035)

## Educación
* Grado Universitario: Ingeniería Mecánica
* Diploma B1 por la ULL
### Cursos
- [x] Redes de Media y Alta Tensión
- [x] Diseño y mantenimiento de instalaciones fotovoltaicas

## Experiencia Laboral
* Ingeniero Técnico en el departamento de mantenimiento en la empresa Elecnor
## Cita favorita
> Que la fuerza te acompañe
## Código 
``` Arduino
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
