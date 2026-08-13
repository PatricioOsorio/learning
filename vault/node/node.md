---
icon: '🟢'
last_reviewed: 2026-08-13
review_stage: 1
next_review: 2026-08-14
---

# Node.js

📚 Temario

---

## 0️⃣ Bienvenida a Node.js & Setup Pro ⚙️🧰

- 🎯 [[00-que-es-node|Qué es Node.js: Arquitectura monohilo y modelo I/O no bloqueante]]
- 🧪 [[00-instalacion-entorno|Instalación profesional del entorno (NVM, Node LTS, Corepack)]]
- 📦 [[00-tipos-de-proyectos|Tipos de proyectos (CLIs, REST APIs, WebSockets, Workers)]]
- 📁 [[00-estructura-de-proyecto|Estructura de proyecto modular y limpia]]
- 🧬 [[00-ciclo-de-ejecucion|Ciclo de ejecución de un script en Node.js]]
- ✅ [[00-primer-hello-world-ts|Primer "Hello World Real" con TypeScript y tsx]]
- 📌 [[00-buenas-practicas-base|Buenas prácticas base (ESLint, Prettier, .env)]]

---

## 1️⃣ Runtime, Arquitectura Interna y V8 🧠⚡

- 🎯 [[01-motor-v8|Motor V8 a fondo: Call Stack, Memory Heap y JIT Compiler]]
- ⚙️ [[01-libuv-cpp-core|Libuv & C++ Core: I/O Asíncrono y Thread Pool nativo]]
- 🔄 [[01-event-loop-fases|El Event Loop al detalle: Las 6 fases de ejecución]]
- ⏱️ [[01-microtasks-vs-macrotasks|Microtasks vs Macrotasks: process.nextTick vs Promises vs Timers]]
- 🚫 [[01-bloqueo-event-loop|Bloqueo del Event Loop: Diagnóstico y prevención]]
- 🚨 [[01-manejo-global-excepciones|Manejo global de excepciones y cierres limpios]]
- 🚩 [[01-v8-flags-cli|V8 Flags y CLI: Inspección de memoria y banderas]]

---

## 2️⃣ Ecosistema Moderno, Módulos & TypeScript 📦🧩

- 📦 [[02-commonjs-vs-esm|CommonJS (CJS) vs ECMAScript Modules (ESM)]]
- 🛠️ [[02-typescript-setup-node|TypeScript para Node.js: Configuración de tsconfig.json]]
- 🔨 [[02-compiladores-bundlers-backend|Compiladores y Bundlers: tsc, tsup, esbuild, swc, tsx]]
- 🆕 [[02-novedades-nativas-node|Novedades Nativas: TypeScript directo, node:watch, node:test]]
- 🏷️ [[02-path-aliases-package-exports|Path Aliases y Package Exports en package.json]]
- 🛡️ [[02-variables-entorno-zod|Variables de entorno estrictas con Zod]]

---

## 3️⃣ Asincronía Profunda, Events, Buffers & Streams 🌊🔍

- 📣 [[03-event-emitter|Pattern EventEmitter: Eventos nativos y prevención de leaks]]
- 🧱 [[03-buffers-arraybuffers|Buffers & ArrayBuffers: Memoria binaria a bajo nivel]]
- 💧 [[03-streams-fundamentos|Fundamentos de Streams: Readable, Writable, Transform, Duplex]]
- 🚰 [[03-backpressure-streams|Gestión de Backpressure y pipeline de streams]]
- 🧰 [[03-async-local-storage|AsyncLocalStorage: Trazabilidad de contexto asíncrono]]

---

## 4️⃣ Aplicaciones CLI, Procesos e IPC 🖥️🔧

- 🕹️ [[04-proceso-process|Manejo del Proceso (process): argv, stdin/stdout y señales]]
- 🌿 [[04-child-processes|Child Processes: exec, execFile, spawn y fork]]
- 💬 [[04-ipc-comunicacion|Inter-Process Communication (IPC) entre procesos]]
- 🛠️ [[04-clis-profesionales|CLIs Profesionales: Executables binarios, Commander y spinners]]

---

## 5️⃣ Clean Architecture & Domain-Driven Design (DDD) 🏛️📐

- 🧅 [[05-clean-architecture-capas|Capas de Clean Architecture: Entities, Use Cases, Adaptadores]]
- 🔌 [[05-inversion-dependencias|Inversión de Dependencias (DIP) y contenedores DI]]
- 🗄️ [[05-repository-pattern|Repository Pattern e implementación InMemory]]
- ⚠️ [[05-manejo-errores-dominio|Manejo de Errores de Dominio y Result Pattern]]
- 🔄 [[05-refactorizacion-hexagonal|Refactorización Práctica hacia Arquitectura Hexagonal]]

---

## 6️⃣ Estrategias de Testing Riguroso (Unit, Integration & E2E) 🧪🛡️

- 🎯 [[06-frameworks-testing|Frameworks de Testing: Vitest, Jest y node:test]]
- 🎭 [[06-test-doubles|Test Doubles: Mocks, Spies, Stubs y Fakes]]
- 🔴 [[06-tdd-ciclo|TDD (Test-Driven Development): Red-Green-Refactor]]
- 🔗 [[06-integration-testing|Integration Testing con bases de datos en contenedores]]
- 📊 [[06-coverage-metricas|Cobertura de código y métricas de calidad en CI]]

---

## 7️⃣ Servidores Web, HTTP/1.1, HTTP/2, REST APIs & Middlewares 🌐⚡

- 🔌 [[07-servidor-http-nativo|Servidor HTTP Nativo con node:http]]
- 🚀 [[07-http2-nativo|HTTP/2 Nativo: Multiplexación y Server Push]]
- ⚔️ [[07-express-vs-fastify|Express.js vs Fastify: Arquitectura y Rendimiento]]
- 🧱 [[07-middlewares-pipeline|Middlewares, Validación DTO con Zod y Handler Global]]
- 📄 [[07-paginacion-filtros-rest|Paginación por Cursor vs Offset y Filtros REST]]

---

## 8️⃣ Persistencia de Datos, ORMs, Migraciones & Redis 🗄️⚡

- 🐘 [[08-postgresql-pg|PostgreSQL con pg: Connection Pool y Transacciones ACID]]
- 🍃 [[08-mongodb-mongoose|MongoDB con Mongoose: Esquemas, Índices y Agregaciones]]
- 🛠️ [[08-orms-prisma-drizzle|ORMs y Query Builders: Prisma y Drizzle ORM]]
- 🌱 [[08-database-seeding|Database Seeding automatizado]]
- ⚡ [[08-redis-caching|Caching con Redis y estrategia Cache-Aside]]

---

## 9️⃣ Autenticación, Autorización & Seguridad Avanzada 🔐🛡️

- 🔑 [[09-hashing-passwords|Hashing seguro de contraseñas: Argon2id y bcrypt]]
- 🎟️ [[09-jwt-autenticacion|Autenticación JWT y Refresh Tokens con Rotación]]
- 🛡️ [[09-autorizacion-rbac-abac|Autorización RBAC / ABAC en Middlewares]]
- 🧱 [[09-owasp-top-10-node|OWASP Top 10 para Node.js, Helmet y Rate Limiting]]
- 🔐 [[09-criptografia-nativo|Criptografía Nativa con node:crypto]]

---

## 🔟 WebSockets & Comunicaciones en Tiempo Real ⚡💬

- 🔌 [[10-protocolo-websocket-nativo|Protocolo WebSocket Nativo: Handshake y Frames]]
- 📡 [[10-socketio-vs-ws|Socket.io vs ws: Servidores en tiempo real y rooms]]
- 🌐 [[10-escalado-websockets-redis|Escalado Horizontal de WebSockets con Redis Pub/Sub]]
- 🔄 [[10-arquitectura-hibrida-realtime|Arquitectura Híbrida: REST + Eventos Real-time]]

---

## 1️⃣1️⃣ Webhooks, Task Queues & Mensajería 🪝📫

- 🪝 [[11-diseno-webhooks|Diseño y consumo de Webhooks asíncronos]]
- 🔒 [[11-seguridad-webhooks-hmac|Seguridad de Webhooks con firmas HMAC (SHA-256)]]
- 📥 [[11-background-queues-bullmq|Background Queues con BullMQ y Redis]]
- 🔁 [[11-resiliencia-queues-dlq|Resiliencia en Filas: Reintentos, Backoff y DLQ]]
- 📮 [[11-message-brokers-rabbitmq-kafka|Message Brokers: RabbitMQ y Apache Kafka (EDA)]]

---

## 1️⃣2️⃣ Concurrencia Avanzada, Worker Threads & Cluster 🧵⚡

- 🔄 [[12-cluster-module|Escalado vertical con el módulo Cluster y Round-Robin]]
- 🧵 [[12-worker-threads|Worker Threads (node:worker_threads) y SharedArrayBuffer]]
- ⚖️ [[12-cluster-vs-workers-vs-child|Comparativa: Cluster vs Workers vs Child Processes]]
- ☁️ [[12-edge-functions-serverless|Edge Functions y Serverless con Node.js]]

---

## 1️⃣3️⃣ Profiling, Memory Leaks & Performance Tuning 📈🔍

- 🔍 [[13-profiling-cpu-flamegraphs|Profiling de CPU con DevTools e inspección de Flamegraphs]]
- 🧹 [[13-memory-leaks-heapdump|Diagnóstico de Memory Leaks con Heap Snapshots]]
- ⏱️ [[13-metricas-event-loop|Latencia del Event Loop con node:perf_hooks]]
- 🚀 [[13-benchmarking-autocannon-k6|Benchmarking y pruebas de carga con Autocannon y k6]]

---

## 1️⃣4️⃣ Dockerización, Observabilidad & DevOps Pro 🐳🚀

- 🐳 [[14-docker-multi-stage|Docker Multi-Stage Builds e imágenes Distroless]]
- 🛑 [[14-graceful-shutdown|Graceful Shutdown con señales SIGTERM y SIGINT]]
- 📝 [[14-structured-logging-pino|Structured Logging JSON de alto rendimiento con Pino]]
- 📊 [[14-opentelemetry-prometheus|Métricas Prometheus y Trazado con OpenTelemetry]]
- 🚀 [[14-orquestacion-pm2-k8s|Orquestación de procesos con PM2 y Kubernetes]]
