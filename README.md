# Notas Estudiantiles

Portal de notas para un salon de clase: la profesora carga materias, alumnos y calificaciones, y cada alumno inicia sesion para ver solo sus propias notas.

Es una sola pagina (index.html) hecha con React + Tailwind, cargados desde CDN, sin proceso de build. Los datos se guardan en Firebase Firestore.

## Paso 1: Crear proyecto en Firebase (gratis, ~5 minutos)

1. Ve a https://console.firebase.google.com
2. 2. Clic en Agregar proyecto, ponle un nombre (ej. notas-clase) y sigue los pasos.
   3. 3. En el menu lateral entra a Firestore Database, Crear base de datos, elige modo de prueba y selecciona una ubicacion cercana.
      4. 4. En el menu lateral ve a Configuracion del proyecto (icono de engranaje), baja hasta Tus apps, clic en el icono </> (Web) y registra la app.
         5. 5. Firebase te mostrara un objeto firebaseConfig con apiKey, projectId, etc. Copia ese bloque completo.
           
            6. ## Paso 2: Pegar la configuracion en index.html
           
            7. 1. Abre index.html en este repositorio (o edita el archivo directamente en GitHub).
               2. 2. Busca el bloque const firebaseConfig cerca del inicio del archivo.
                  3. 3. Reemplazalo por el bloque que copiaste de Firebase.
                     4. 4. Guarda y confirma el cambio (commit).
                       
                        5. ## Paso 3: Desplegar
                       
                        6. Este repositorio esta conectado a Vercel. Cada cambio en la rama main se despliega automaticamente.
                       
                        7. ## Importante sobre seguridad
                       
                        8. El modo de prueba de Firestore deja la base de datos abierta por 30 dias (despues hay que ajustar las reglas). Es suficiente para un salon de clase, pero no es seguridad de nivel bancario: cualquiera con el link de la app tecnicamente podria intentar entrar. Las contrasenas se guardan en texto simple, no cifradas.
                       
                        9. Si mas adelante se quiere reforzar la seguridad, se puede agregar Firebase Authentication.
                        10. 
