# 🏆 DESAFÍO AWS: Portfolio Personal

**"Construye tu Portfolio Profesional en la Nube"**

---

## 🎯 CONCEPTO DEL DESAFÍO

### Fase 1: Desarrollo 
**Opción 1**
**Todos juntos enfocados en hacer backend con AWS** construimos un **template de portfolio** con:
**- Frontend:**
```
Páginas principales:
├── Home (Hero + resumen)
├── About (perfil detallado)
├── Projects (galería de proyectos)
├── Contact (formulario + info)
└── Admin (panel para editar datos)
```

**- Backend:** realizado con servicios extras de AWS
```
├── API Gateway (REST API)
├── Lambda Functions (Node.js)
└── DynamoDB (2 tablas)
```
- Base de datos para perfil y proyectos
- Autenticación básica
**Opción 2**
**Individual usando su propio Stack** debe contruir un **Portfolio web** con:
- Frontend responsive con:
```
Páginas principales:
├── Home (Hero + resumen)
├── About (perfil detallado)
├── Projects (galería de proyectos)
├── Contact (formulario + info)
└── Admin (panel para editar datos)
```
**- Backend:** realizado en base a stack del participante pero desplegado en AWS
- Base de datos para perfil y proyectos


Nota: Indiferentemente de la opción seleccionada deben usar este repositorio para el desafio, si la opcion es trabajar en:
**Colaborativo** deben trabajar de manera ordenada con pull request y son libres de crear las ramas necesarias segun lo que esten trabajando.
**Individual** deben hacer un fork de este github y trabajarlo en base a la estructura

### Fase 2: Competencia Individual
**Cada participante** toma el template y:
- Lo personaliza con su información y modificación en base a su estructura backend
- Lo despliega en AWS con su propia arquitectura
- Compite por el mejor deployment y personalización

Nota: Indiferentemente de la opción seleccionada en la fase 1 la fase 2 va a ser igual. Todos tenemos que adaptar el template al backend que querramos hacer, ya sea con un stack distinto a aws

### Fase 3: Competencia Individual **Opcional**
**QUEDARA PENDIENTE DE EVALUACIÓN DE FASE 1 Y 2**

---

## 📋 ESTRUCTURA DEL TEMPLATE

### 🎨 Frontend: Portfolio web
```
Páginas principales:
├── Home (Hero + resumen)
├── About (perfil detallado)
├── Projects (galería de proyectos)
├── Contact (formulario + info)
└── Admin (panel para editar datos)
```

### ⚡ Backend: API REST
```
Endpoints principales:
├── GET /api/profile (datos del usuario)
├── PUT /api/profile (actualizar perfil)
├── GET /api/projects (lista de proyectos)
├── POST /api/projects (crear proyecto)
├── PUT /api/projects/:id (editar proyecto)
└── DELETE /api/projects/:id (eliminar proyecto)
```

**Nota:** Ideal si crean un portal de autenticacion y sus apis asociadas

### 🗄️ Base de Datos: Estructura Simple
```
Tabla: user_profile
├── id (string)
├── name (string)
├── title (string)
├── bio (text)
├── email (string)
├── phone (string)
├── location (string)
├── skills (array)
├── social_links (object)
└── profile_image_url (string)

Tabla: projects
├── id (string)
├── user_id (string)
├── title (string)
├── description (text)
├── tech_stack (array)
├── github_url (string)
├── live_url (string)
├── image_url (string)
├── featured (boolean)
└── created_at (timestamp)
```

---

## 🛠️ ESPECIFICACIONES TÉCNICAS

### Arquitectura AWS 
```
Frontend:
└── S3 Bucket (Static Website) + CloudFront

Backend:
├── API Gateway (REST API)
├── Lambda Functions (Node.js)
└── DynamoDB (2 tablas)

Opcional:
├── ACM (certificado SSL)               #Si es que se puede
└── S3 (para imágenes de proyectos)     #Ideal
```

---

## 🏆 CRITERIOS DE COMPETENCIA (Fase 2)

### 📊 Evaluación Individual (100 puntos)

| Criterio | Puntos | Descripción |
|----------|--------|-------------|
| **Deployment Exitoso** | 25 pts | ¿La app funciona en AWS sin errores? |
| **Personalización** | 20 pts | ¿Qué tan bien adaptaste el template?    |
| **Arquitectura AWS** | 20 pts | Uso eficiente de servicios             |
| **Contenido** | 10 pts | Calidad de proyectos y perfil                 |
y otros criterios...


## 🎁 PREMIOS

### 🥇 Primer premio - **3 recomendaciones en LinkedIn** corroborando experiencia en alguna de las tecnologías o herramientas ocupadas en este desafío.

### 🥇 Segundo premio -**Ayuda con despliegue de portafolio en dominio .is-a.dev** para desplegar portafolio solo en front con github pages

> **Nota**: Dado que no tenemos presupuesto para premios, estos son los mejores premios que se me ocurrieron.

---

## 📦 ENTREGABLES

### Durante Desarrollo Colaborativo:
- **Commits diarios** en repositorio común
- **Testing** de cada feature antes de merge
- **Documentación** de APIs y componentes

### Para el Desafío:
1. **URL del portfolio** funcionando en el video
2. **Repositorio GitHub** personalizado 
3. **Video demo** de 2 minutos mostrando:
   - Portfolio navegable
   - Panel de admin funcionando
   - Explicación de arquitectura AWS
4. **Documento técnico** explicando:
   - Servicios AWS utilizados
   - Decisiones de arquitectura
   - Optimizaciones implementadas

---

## 💡 ESTRUCTURA DE REPOSITORIO

```
desafio-aws-portafolio/
├── frontend/
│   ├── 
├── backend/
│   ├── 
├── infrastructure/   #En caso de tener archivos de infraestructura
│   ├──
└── docs/
    ├── API.md
    ├── DEPLOYMENT.md
    └── CUSTOMIZATION.md
```

---

## 🚀 VENTAJAS DE ESTA APROXIMACIÓN

### 🤝 Colaborativa
- Todos aprenden la misma arquitectura
- Código de calidad revisado por el grupo
- Conocimiento compartido

### 🎯 Práctica
- Portfolio real para uso profesional
- Experiencia completa de development + ops
- Proyecto para mostrar a empleadores

### 🏁 Competitiva
- Motivación personal en deployment
- Cada uno demuestra sus habilidades únicas
- Comparación directa de implementaciones

### 💼 Profesional
- URL permanente para CV
- Evidencia tangible de skills AWS
- Template reutilizable para futuros proyectos

---

## 📞 SOPORTE DURANTE EL DESAFÍO
---

El soporte será brindado por cada uno de nosotros en el **Grupo de WhatsApp** o por **Discord** 
https://discord.gg/853rH9zt


## 📝 POLÍTICAS PARA PARTICIPAR

### ⚖️Compromiso
- Al participar entras entre un sorteo, los seleccionados del sorteo tendran que dar una buena recomendación en Linkedin al ganador del Desafío
- Al participar en este desafio te comprometes a participar hasta el final - COMPROMISO!
  
### ✅ Permitido
- Usar código de tutoriales como base
- Colaborar en ideas y debugging
- Usar librerías y frameworks públicos
- Buscar soluciones en Stack Overflow/Google
- Usar cualquier editor de codigo
- Usar cualquier IA.
- Puedes agregar mas columnas en las tablas solicitadas
- Puedes agregar mas tablas

### ❌ No Permitido
- Copiar código completo de otros participantes
- Usar servicios de AWS que no abarque el Test Lab del Bootcamp
- Presentar trabajo de terceros como propio
- Modificar fecha de commits para aparentar más trabajo
- Modificar estructura de apis solicitadas o bases de datos

### 🚨 Penalizaciones
- **Copia**: Descalificación inmediata
- **Entrega tarde**: -10 puntos por cada hora de retraso
- **App no funcional**: -50 puntos

**Descalificacion inmediata** si no cumples con: 
**Colaborativo** deben trabajar de manera ordenada con pull request y son libres de crear las ramas necesarias segun lo que esten trabajando.
**Individual** deben hacer un fork de este github y trabajarlo en base a la estructura

---

## 🎉 ¡A CODEAR SE HA DICHO!

**Objetivo**: Al final, cada participante tendrá su portfolio profesional desplegado en AWS, con código de calidad y una sólida comprensión de arquitectura en la nube.

**¡Que comience el desarrollo colaborativo!** 🚀

---

## 🤝 Contribuidores

[Owensl](https://github.com/OwensLopez211)


## 📄 Licencia



## 🙏 Agradecimientos

- Comunidad AWS por los recursos gratuitos
- Participantes del bootcamp Generation Chile Cohorte 6 por la colaboración
- Mentores por el apoyo técnico
