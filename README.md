# Convertidor DOC a PDF

Una aplicación web simple para convertir documentos de Word (.doc, .docx) a PDF.

## Requisitos

- Python 3.x
- Flask
- python-docx
- pdfkit
- wkhtmltopdf

## Instalación

Las dependencias ya están instaladas en este entorno. Si necesitas instalarlas manualmente:

```bash
pip install flask python-docx pdfkit
apt-get install -y wkhtmltopdf
```

## Uso

1. Inicia el servidor:
```bash
python app.py
```

2. Abre tu navegador y ve a: `http://localhost:5000`

3. Sube un archivo .doc o .docx y haz clic en "Convertir a PDF"

4. El archivo PDF se descargará automáticamente

## Características

- Interfaz moderna y responsive
- Soporte para arrastrar y soltar archivos
- Conversión de .docx usando python-docx
- Conversión de .doc antiguos (requiere LibreOffice)
- Descarga automática del PDF convertido
- Manejo de errores y validación de archivos

## Estructura del proyecto

```
/workspace
├── app.py          # Servidor Flask con la lógica de conversión
├── index.html      # Interfaz de usuario
└── README.md       # Este archivo
```

## Notas

- Los archivos .docx se convierten primero a HTML y luego a PDF
- Los archivos .doc antiguos requieren LibreOffice instalado
- Los archivos temporales se eliminan automáticamente después de la conversión
