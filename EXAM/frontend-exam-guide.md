# FRONTEND EXAM GUIDE / GUÍA EXAMEN FRONTEND
## React + TypeScript + Official Documentation / Documentación Oficial

---

# 🧠 EXAM MENTAL PATTERN / PATRÓN MENTAL PARA EL EXAMEN

| The prompt says / El enunciado dice | Use / Usa |
|---|---|
| form / formulario | RHF + Zod + zodResolver |
| validation / validación | Zod schema + refine |
| API / server data / datos del servidor | TanStack Query useQuery |
| create / edit / delete / crear / editar / borrar | TanStack Query useMutation |
| navigation / navegación | React Router |
| global state / estado global | Zustand |
| cart / auth / carrito / autenticación | Zustand store |
| quick styles / estilos rápidos | TailwindCSS |
| ready components / componentes listos | Chakra UI o MUI |
| data table / tabla con datos | MUI DataGrid o map() |
| test logic / probar lógica | Jest |
| test component / probar componente | React Testing Library |
| test full flow / probar flujo completo | Cypress |

---

# 📦 INSTALLATIONS / INSTALACIONES

| Topic / Tema | Command / Comando |
|---|---|
| Base project / Proyecto base | `npm create vite@latest mi-proyecto -- --template react-ts` |
| React Router | `npm install react-router-dom` |
| TanStack Router | `npm install @tanstack/react-router` |
| TanStack Router Plugin | `npm install --save-dev @tanstack/router-plugin` |
| React Hook Form | `npm install react-hook-form` |
| RHF + Zod resolver | `npm install @hookform/resolvers` |
| Formik | `npm install formik` |
| Yup | `npm install yup` |
| Zod | `npm install zod` |
| Zustand | `npm install zustand` |
| MobX | `npm install mobx mobx-react-lite` |
| TanStack Query | `npm install @tanstack/react-query` |
| TanStack Query Devtools | `npm install @tanstack/react-query-devtools` |
| TailwindCSS | `npm install tailwindcss @tailwindcss/vite` |
| Clsx | `npm install clsx` |
| Chakra UI | `npm install @chakra-ui/react` |
| Material UI | `npm install @mui/material @emotion/react @emotion/styled` |
| MUI Icons | `npm install @mui/icons-material` |
| Jest | `npm install --save-dev jest @types/jest ts-jest` |
| RTL | `npm install --save-dev @testing-library/react @testing-library/jest-dom @testing-library/user-event jest-environment-jsdom` |
| Cypress | `npm install --save-dev cypress` |

## All in one / Todo en uno
```bash
# Create project / Crear proyecto
npm create vite@latest mi-examen -- --template react-ts
cd mi-examen && npm install

# Main libraries / Librerías principales
npm install react-router-dom @tanstack/react-query @tanstack/react-query-devtools react-hook-form zod @hookform/resolvers zustand

# UI — choose one / elige una
npm install tailwindcss @tailwindcss/vite clsx
# or / o
npm install @chakra-ui/react
# or / o
npm install @mui/material @emotion/react @emotion/styled @mui/icons-material

# Testing
npm install --save-dev jest @types/jest ts-jest @testing-library/react @testing-library/jest-dom @testing-library/user-event jest-environment-jsdom cypress
```

---

# 🔑 KEYWORDS / PALABRAS CLAVE

## React / TypeScript / Hooks
```
ES: componente, props, estado, efecto, referencia, contexto, hooks, interfaz, tipo, genéricos
EN: component, props, state, effect, ref, context, hooks, interface, type, generics,
    React.ChangeEvent, React.MouseEvent, React.FormEvent
```

## React Router
```
ES: enrutador, rutas, enlace, navegar, parámetros
EN: BrowserRouter, Routes, Route, Link, useNavigate, useParams, Outlet, nested routes
```

## React Hook Form
```
ES: formulario, registro, envío, errores, controlador
EN: useForm, register, handleSubmit, formState, errors, isSubmitting,
    reset, setError, zodResolver, Controller, watch
```

## Formik
```
ES: valores iniciales, envío, validación, tocado, errores
EN: useFormik, initialValues, onSubmit, validate, validationSchema,
    touched, errors, handleChange, handleBlur, Field, Form, ErrorMessage
```

## Zod
```
ES: esquema, objeto, cadena, número, analizar, refinar, inferir
EN: z.object, z.string, z.number, z.boolean, z.array, safeParse,
    parse, refine, z.infer, min, max, email, nonempty, optional, nullable
```

## Zustand
```
ES: crear, establecer, obtener, selector, persistir
EN: create, set, get, subscribe, selector, shallow, persist, middleware, devtools
```

## MobX
```
ES: observable, acción, computado, observador, reacción
EN: makeAutoObservable, observable, action, computed, observer, reaction, autorun
```

## TanStack Query
```
ES: cliente, consulta, mutación, clave, invalidar, pendiente
EN: QueryClient, QueryClientProvider, useQuery, useMutation, useQueryClient,
    queryKey, queryFn, enabled, staleTime, invalidateQueries, onSuccess, isPending
```

## TailwindCSS
```
ES: flex, cuadrícula, relleno, margen, fondo, texto, borde, sombra, responsivo
EN: flex, grid, padding, margin, background, text, border, rounded,
    shadow, hover, focus, responsive, sm: md: lg: xl:, gap, width, height
```

## Chakra UI
```
ES: proveedor, caja, pila, botón, entrada, campo, diálogo, notificación
EN: Provider, Box, Flex, Grid, HStack, VStack, Button, Input,
    Field, Dialog, Toaster, Badge, Spinner
```

## Material UI
```
ES: caja, pila, cuadrícula, botón, campo de texto, tipografía, barra de app
EN: Box, Stack, Grid, Button, TextField, Typography, AppBar, Card,
    Dialog, Snackbar, Chip, CircularProgress, sx, variant, color, Controller
```

## Jest
```
ES: describir, prueba, esperar, comparador, simulación, configuración
EN: describe, test, it, expect, toBe, toEqual, toContain, toThrow,
    beforeEach, afterEach, jest.fn, jest.mock, mockResolvedValue
```

## React Testing Library
```
ES: renderizar, pantalla, disparar evento, usuario, consulta, afirmación
EN: render, screen, fireEvent, userEvent, getByText, getByRole,
    getByLabelText, queryByText, findByText, toBeInTheDocument, toHaveTextContent
```

## Cypress
```
ES: visitar, obtener, contiene, hacer clic, escribir, afirmar, interceptar
EN: cy.visit, cy.get, cy.contains, cy.click, cy.type, cy.should,
    cy.url, cy.intercept, cy.wait, data-testid, Cypress.Commands.add
```

---

# 📄 DOCUMENT NAMES / NOMBRES DE DOCUMENTOS

## React
| English | Español |
|---|---|
| Your First Component | Tu primer componente |
| Passing Props to a Component | Pasar props a un componente |
| Conditional Rendering | Renderizado condicional |
| Rendering Lists | Renderizar listas |
| Responding to Events | Responder a eventos |
| State: A Component's Memory | Estado: la memoria de un componente |
| Synchronizing with Effects | Sincronizar con efectos |
| Referencing Values with Refs | Referenciar valores con refs |
| Manipulating the DOM with Refs | Manipular el DOM con refs |
| Passing Data Deeply with Context | Pasar datos profundamente con contexto |
| Updating Objects in State | Actualizar objetos en el estado |
| Updating Arrays in State | Actualizar arrays en el estado |
| Queueing a Series of State Updates | Encolar una serie de actualizaciones |
| You Might Not Need an Effect | Puede que no necesites un efecto |

## TypeScript
| English | Español |
|---|---|
| TypeScript Overview | Descripción general de TypeScript |
| Typing Component Props | Tipar props de componentes |
| Typing useState | Tipar useState |
| Typing DOM Events | Tipar eventos del DOM |
| Everyday Types | Tipos cotidianos |

## React Router
| English | Español |
|---|---|
| Installation | Instalación |
| Routing | Enrutamiento |
| Navigating | Navegación |
| URL Params | Parámetros de URL |
| Nested Routes | Rutas anidadas |
| 404 Routes | Ruta 404 |

## TanStack Router
| English | Español |
|---|---|
| Quick Start | Inicio rápido |
| File Based Routing | Enrutamiento basado en archivos |
| Route Params | Parámetros de ruta |
| Navigation | Navegación |
| Router Context | Contexto del router |

## React Hook Form
| English | Español |
|---|---|
| Get Started | Comenzar |
| useForm API | API de useForm |
| register | Registrar campos |
| formState | Estado del formulario |
| handleSubmit | Manejar envío |
| setError | Establecer error |
| Controller | Controlador |
| Schema Validation | Validación con schema |

## Formik
| English | Español |
|---|---|
| Overview | Descripción general |
| useFormik | useFormik |
| Validation | Validación |
| Schema Validation with Yup | Validación con Yup |
| Field | Campo |
| ErrorMessage | Mensaje de error |
| The Formik Component | El componente Formik |

## Zod
| English | Español |
|---|---|
| Basic Usage | Uso básico |
| Primitives | Primitivos |
| Objects | Objetos |
| Strings | Cadenas de texto |
| Numbers | Números |
| Arrays | Arreglos |
| Unions | Uniones |
| Refine | Refinamiento |
| Error Handling | Manejo de errores |
| Type Inference | Inferencia de tipos |

## Zustand
| English | Español |
|---|---|
| Introduction | Introducción |
| Updating State | Actualizar estado |
| TypeScript Guide | Guía de TypeScript |
| Selecting Multiple State Slices | Seleccionar múltiples partes del estado |
| Persisting Store Data | Persistir datos del store |
| Devtools Middleware | Middleware de devtools |

## MobX
| English | Español |
|---|---|
| The Gist of MobX | La esencia de MobX |
| Observable State | Estado observable |
| makeAutoObservable | makeAutoObservable |
| Actions | Acciones |
| Computeds | Valores computados |
| Reactions | Reacciones |
| React Integration | Integración con React |
| Observer | Observer |

## TanStack Query
| English | Español |
|---|---|
| Quick Start | Inicio rápido |
| Queries | Consultas |
| Query Keys | Claves de consulta |
| Query Functions | Funciones de consulta |
| Mutations | Mutaciones |
| Query Invalidation | Invalidación de consultas |
| Dependent Queries | Consultas dependientes |
| Paginated Queries | Consultas paginadas |
| useQuery Reference | Referencia de useQuery |
| useMutation Reference | Referencia de useMutation |

## TailwindCSS
| English | Español |
|---|---|
| Installation: Using Vite | Instalación con Vite |
| Flex | Flexbox |
| Grid Template Columns | Columnas de cuadrícula |
| Padding | Relleno |
| Margin | Margen |
| Background Color | Color de fondo |
| Text Color | Color de texto |
| Border Radius | Radio de borde |
| Box Shadow | Sombra de caja |
| Responsive Design | Diseño responsivo |
| Hover, Focus and Other States | Estados hover, focus y otros |
| Dark Mode | Modo oscuro |

## Chakra UI
| English | Español |
|---|---|
| Installation | Instalación |
| Box | Caja |
| Stack / HStack / VStack | Pila / Pila horizontal / Pila vertical |
| Button | Botón |
| Input | Entrada |
| Field | Campo |
| Dialog | Diálogo |
| Toaster | Notificaciones |
| Badge | Insignia |
| Spinner | Indicador de carga |
| Alert | Alerta |

## Material UI
| English | Español |
|---|---|
| Installation | Instalación |
| Button | Botón |
| Text Field | Campo de texto |
| Typography | Tipografía |
| Grid | Cuadrícula |
| Stack | Pila |
| Box | Caja |
| App Bar | Barra de aplicación |
| Card | Tarjeta |
| Dialog | Diálogo |
| Snackbar | Barra de notificación |
| Chip | Etiqueta |
| Circular Progress | Progreso circular |
| Table | Tabla |
| Data Grid | Cuadrícula de datos |
| The sx prop | La prop sx |

## Jest
| English | Español |
|---|---|
| Getting Started | Comenzar |
| Using Matchers | Usar comparadores |
| Testing Asynchronous Code | Probar código asíncrono |
| Setup and Teardown | Configuración y desmontaje |
| Mock Functions | Funciones simuladas |
| Jest Object | Objeto Jest |
| Expect API | API de Expect |
| Timer Mocks | Temporizadores simulados |

## React Testing Library
| English | Español |
|---|---|
| Introduction | Introducción |
| Queries | Consultas |
| ByRole | Por rol |
| ByText | Por texto |
| ByLabelText | Por etiqueta |
| ByTestId | Por ID de prueba |
| Firing Events | Disparar eventos |
| Async Utilities | Utilidades asíncronas |
| User Interactions | Interacciones de usuario |
| jest-dom Custom Matchers | Comparadores de jest-dom |

## Cypress
| English | Español |
|---|---|
| Writing Your First E2E Test | Escribir tu primer test E2E |
| Interacting with Elements | Interactuar con elementos |
| Assertions | Afirmaciones |
| Network Requests | Solicitudes de red |
| cy.intercept | cy.intercept |
| cy.get | cy.get |
| cy.contains | cy.contains |
| cy.visit | cy.visit |
| Custom Commands | Comandos personalizados |
| Best Practices | Mejores prácticas |
| Fixtures | Fixtures |

---

# 🔍 WHAT TO SEARCH ON GOOGLE / QUÉ ESCRIBIR EN GOOGLE

| Topic / Tema | Google |
|---|---|
| React | `react.dev` |
| TypeScript | `typescriptlang.org` |
| React Router | `reactrouter.com` |
| TanStack Router | `tanstack.com router` |
| React Hook Form | `react-hook-form.com` |
| Formik | `formik.org` |
| Zod | `zod.dev` |
| Zustand | `zustand docs` |
| MobX | `mobx.js.org` |
| TanStack Query | `tanstack.com query` |
| TailwindCSS | `tailwindcss.com docs` |
| Chakra UI | `chakra-ui.com docs` |
| Material UI | `mui.com` |
| Jest | `jestjs.io docs` |
| React Testing Library | `testing-library.com` |
| Cypress | `docs.cypress.io` |

---

# 💡 EXAM TRICK / TRUCO PARA EL EXAMEN

```
EN:
1. Open the topic base URL on Google
2. Use Ctrl+F to search for the function or component
3. Read only the minimal example
4. Copy the pattern and adapt it

If you can't find it fast, search on Google like:
→ react useEffect example
→ zod refine two fields
→ mui textfield error react hook form
→ tanstack query invalidate cache
→ zustand typescript example

ES:
1. Abre la URL base del tema en Google
2. Usa Ctrl+F para buscar la función o componente
3. Lee solo el ejemplo mínimo
4. Copia el patrón y adáptalo

Si no encuentras rápido, busca en Google así:
→ react useEffect ejemplo
→ zod refine dos campos
→ mui textfield error react hook form
→ tanstack query invalidate cache
→ zustand typescript ejemplo
```
