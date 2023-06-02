Infraestructura como Código con Terraform


Este repositorio contiene el código de infraestructura como código (IaC) utilizado para implementar y administrar la infraestructura en la nube utilizando Terraform. Con Terraform, podemos describir y versionar nuestra infraestructura de manera declarativa, lo que nos permite tener un control preciso sobre nuestros recursos en la nube.

Estructura del Repositorio
El repositorio está organizado de la siguiente manera:

bash
Copy code
├── .github
│   └── workflows
│       └── pipeline.yml
├── terraform
│   ├── main.tf
│   ├── variables.tf
│   └── .env
└── README.md
El directorio .github/workflows contiene el archivo pipeline.yml, que define el flujo de trabajo de GitHub Actions utilizado para automatizar el despliegue y la gestión de la infraestructura.
El directorio terraform contiene los archivos principales de Terraform:
main.tf: Define los recursos de AWS utilizados, como instancias de EC2, grupos de seguridad, etc.
variables.tf: Define las variables utilizadas en el código de Terraform, como la región de AWS, el tipo de instancia, etc.
.env: Archivo de entorno que contiene las variables de configuración sensibles, como las credenciales de AWS.
Uso
Clona este repositorio en tu máquina local.

Configura las variables necesarias en el archivo .env según tus credenciales y configuración de AWS.

Ejecuta el siguiente comando para inicializar Terraform:

shell
Copy code
terraform init
Ejecuta el siguiente comando para ver el plan de ejecución de Terraform:

shell
Copy code
terraform plan
Si el plan de ejecución es correcto, ejecuta el siguiente comando para aplicar los cambios:

shell
Copy code
terraform apply -auto-approve
Contribución
Si deseas contribuir a este proyecto, siéntete libre de hacerlo. Puedes enviar tus pull requests y reportar cualquier problema que encuentres. Agradecemos cualquier aporte para mejorar la infraestructura y los flujos de trabajo.

Notas Importantes
Mantén tus credenciales y variables de configuración confidenciales y no las compartas públicamente.
Antes de realizar cambios importantes, asegúrate de entender el impacto que tendrán en la infraestructura existente y realiza pruebas exhaustivas.