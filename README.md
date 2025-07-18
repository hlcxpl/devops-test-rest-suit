# 🚀 DevOps Test REST Suite

Automatización de pruebas REST utilizando **SoapUI** y un enfoque integrable en pipelines DevOps.

---

## 📋 Descripción

Este repositorio contiene una suite de pruebas funcionales para APIs REST, creada con **SoapUI**. Ideal para:

- Verificar endpoints REST y validar respuestas.
- Integración en CI/CD con Jenkins, GitHub Actions o similares.
- Compatibilidad multiplataforma (Windows, Linux, macOS).

---

## 🎯 Características clave

- Casos de prueba definidos en formato `.xml` de SoapUI.
- Aserciones para validar status codes, esquemas JSON/XML, contenido.
- Ejecución en modo headless para integración automatizada.
- Facilita pruebas funcionales antes o después del despliegue.

---

## 🛠️ Prerrequisitos

- [SoapUI Open Source](https://www.soapui.org/downloads/) (o ReadyAPI).
- **Java 8+** instalado en la máquina.
- Acceso al endpoint REST que deseas probar.

---

## 🚧 Cómo ejecutar las pruebas

1. Clona el repositorio:
   ```bash
   git clone https://github.com/hlcxpl/devops-test-rest-suit.git
   cd devops-test-rest-suit
   ```

2. Abre `Project-1-soapui-project.xml` en SoapUI y ejecuta la suite manualmente; o bien:

3. Ejecución desde línea de comando (usando testrunner.sh):
   ```bash
   ./SoapUI/bin/testrunner.sh -s"Test_Suit_1" -r -j -f reports Project-1-soapui-project.xml
   ```

---

## 🔁 Integración en CI/CD

| CI/CD Tool       | Instrucciones                                          |
|------------------|--------------------------------------------------------|
| **Jenkins**      | Plugins: Maven, JUnit; ejecutar script con SoapUI CLI |
| **GitHub Actions** | Usa acción que instale Java + SoapUI CLI; luego ejecuta testrunner |

---

## 🧪 Estructura del Proyecto

```
devops-test-rest-suit/
├── Project-1-soapui-project.xml   # Suite de pruebas REST
├── README.md                      # Documentación del proyecto
└── reports/                       # Resultados de pruebas generados por SoapUI
    └── TEST-Test_Suit_1.xml
```

---

## 📝 Licencia

Este proyecto está disponible bajo la **licencia MIT**. Consulta el archivo `LICENSE` si lo deseas incluir.

---

## 🤝 Autor

**Luis Sánchez**  
📫 Contacto: hlcxpl@gmail.com  
GitHub: [hlcxpl](https://github.com/hlcxpl)
