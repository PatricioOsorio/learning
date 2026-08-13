---
icon: '🟢'
last_reviewed: 2026-08-13
review_stage: 1
next_review: 2026-08-14
---

# Node.js

📚 Temario

---

## 0️⃣ Bienvenida a Node.js & Setup Pro ⚙️

- 🎯 [[01-que-es-node|Qué es Node.js: Arquitectura monohilo y modelo I/O no bloqueante]]
- 🧪 [[02-instalacion-entorno|Instalación profesional del entorno (NVM, Node LTS, Corepack)]]
- 📦 [[03-tipos-de-proyectos|Tipos de proyectos (CLIs, REST APIs, WebSockets, Workers)]]
- 📁 [[04-estructura-de-proyecto|Estructura de proyecto modular y limpia]]
- 🧬 [[05-ciclo-de-ejecucion|Ciclo de ejecución de un script en Node.js]]
- ✅ [[06-primer-hello-world-ts|Primer "Hello World Real" con TypeScript y tsx]]
- 📌 [[07-buenas-practicas-base|Buenas prácticas base (ESLint, Prettier, .env)]]

---

## 1️⃣ Runtime, Arquitectura Interna y V8 🧠⚡

- 🎯 [[01-motor-v8|Motor V8 a fondo: Call Stack, Memory Heap y JIT Compiler]]
- ⚙️ [[02-libuv-cpp-core|Libuv & C++ Core: I/O Asíncrono y Thread Pool nativo]]
- 🔄 [[03-event-loop-fases|El Event Loop al detalle: Las 6 fases de ejecución]]
- ⏱️ [[04-microtasks-vs-macrotasks|Microtasks vs Macrotasks: process.nextTick vs Promises vs Timers]]
- 🚫 [[05-bloqueo-event-loop|Bloqueo del Event Loop: Diagnóstico y prevención]]
- 🚨 [[06-manejo-global-excepciones|Manejo global de excepciones y cierres limpios]]
- 🚩 [[07-v8-flags-cli|V8 Flags y CLI: Inspección de memoria y banderas]]

---

## 2️⃣ Ecosistema Moderno, Módulos & TypeScript 📦🧩

- 📦 [[01-commonjs-vs-esm|CommonJS (CJS) vs ECMAScript Modules (ESM)]]
- 🛠️ [[02-typescript-setup-node|TypeScript para Node.js: Configuración de tsconfig.json]]
- 🔨 [[03-compiladores-bundlers-backend|Compiladores y Bundlers: tsc, tsup, esbuild, swc, tsx]]
- 🆕 [[04-novedades-nativas-node|Novedades Nativas: TypeScript directo, node:watch, node:test]]
- 🏷️ [[05-path-aliases-package-exports|Path Aliases y Package Exports en package.json]]
- 🛡️ [[06-variables-entorno-zod|Variables de entorno strictly con Zod]]

---

## 3️⃣ Asincronía Profunda, Events, Buffers & Streams 🌊🔍

- 📣 [[01-event-emitter|Pattern EventEmitter: Eventos nativos y prevención de leaks]]
- 🧱 [[02-buffers-arraybuffers|Buffers & ArrayBuffers: Memoria binaria a bajo nivel]]
- 💧 [[03-streams-fundamentos|Fundamentos de Streams: Readable, Writable, Transform, Duplex]]
- 🚰 [[04-backpressure-streams|Gestión de Backpressure y pipeline de streams]]
- 🧰 [[05-async-local-storage|AsyncLocalStorage: Trazabilidad de contexto asíncrono]]

---

## 4️⃣ Aplicaciones CLI, Procesos e IPC 🖥️🔧

- 🕹️ [[01-proceso-process|Manejo del Proceso (process): argv, stdin/stdout y señales]]
- 🌿 [[02-child-processes|Child Processes: exec, execFile, spawn y fork]]
- 💬 [[03-ipc-comunicacion|Inter-Process Communication (IPC) entre procesos]]
- 🛠️ [[04-clis-profesionales|CLIs Profesionales: Executables binarios, Commander y spinners]]

---

## 5️⃣ Clean Architecture & Domain-Driven Design (DDD) 🏛️📐

- 🧅 [[01-clean-architecture-capas|Capas de Clean Architecture: Entities, Use Cases, Adaptadores]]
- 🔌 [[02-inversion-dependencias|Inversión de Dependencias (DIP) y contenedores DI]]
- 🗄️ [[03-repository-pattern|Repository Pattern e implementación InMemory]]
- ⚠️ [[04-manejo-errores-dominio|Manejo de Errores de Dominio y Result Pattern]]
- 🔄 [[05-refactorizacion-hexagonal|Refactorización Práctica hacia Arquitectura Hexagonal]]

---

## 6️⃣ Estrategias de Testing Riguroso (Unit, Integration & E2E) 🧪🛡️

- 🎯 [[01-frameworks-testing|Frameworks de Testing: Vitest, Jest y node:test]]
- 🎭 [[02-test-doubles|Test Doubles: Mocks, Spies, Stubs y Fakes]]
- 🔴 [[03-tdd-ciclo|TDD (Test-Driven Development): Red-Green-Refactor]]
- 🔗 [[04-integration-testing|Integration Testing con bases de datos en contenedores]]
- 🌐 [[05-e2e-api-testing|Pruebas E2E de APIs HTTP con Supertest y Testcontainers]]
- 📊 [[06-coverage-metricas|Cobertura de código y métricas de calidad en CI]]

---

## 7️⃣ Servidores Web, HTTP/1.1, HTTP/2, REST APIs & Middlewares 🌐⚡

- 🔌 [[01-servidor-http-nativo|Servidor HTTP Nativo con node:http]]
- 🚀 [[02-http2-nativo|HTTP/2 Nativo: Multiplexación y Server Push]]
- ⚔️ [[03-express-vs-fastify|Express.js vs Fastify: Arquitectura y Rendimiento]]
- 🧱 [[04-middlewares-pipeline|Middlewares, Validación DTO con Zod y Handler Global]]
- 📄 [[05-paginacion-filtros-rest|Paginación por Cursor vs Offset y Filtros REST]]

---

## 8️⃣ Persistencia de Datos, ORMs, Migraciones & Redis 🗄️⚡

- 🐘 [[01-postgresql-pg|PostgreSQL con pg: Connection Pool y Transacciones ACID]]
- 🍃 [[02-mongodb-mongoose|MongoDB con Mongoose: Esquemas, Índices y Agregaciones]]
- 🛠️ [[03-orms-prisma-drizzle|ORMs y Query Builders: Prisma y Drizzle ORM]]
- 📜 [[04-migraciones-schema-db|Migraciones de Esquema de Base de Datos y control de versiones]]
- 🌱 [[05-database-seeding|Database Seeding automatizado]]
- ⚡ [[06-redis-caching|Caching con Redis y estrategia Cache-Aside]]

---

## 9️⃣ Autenticación, Autorización & Seguridad Avanzada 🔐🛡️

- 🔑 [[01-hashing-passwords|Hashing seguro de contraseñas: Argon2id y bcrypt]]
- 🎟️ [[02-jwt-autenticacion|Autenticación JWT y Refresh Tokens con Rotación]]
- 🛡️ [[03-autorizacion-rbac-abac|Autorización RBAC / ABAC en Middlewares]]
- 🧱 [[04-owasp-top-10-node|OWASP Top 10 para Node.js, Helmet y Rate Limiting]]
- 🔐 [[05-criptografia-nativo|Criptografía Nativa con node:crypto]]

---

## 🔟 WebSockets & Comunicaciones en Tiempo Real ⚡💬

- 🔌 [[01-protocolo-websocket-nativo|Protocolo WebSocket Nativo: Handshake y Frames]]
- 📡 [[02-socketio-vs-ws|Socket.io vs ws: Servidores en tiempo real y rooms]]
- 🌐 [[03-escalado-websockets-redis|Escalado Horizontal de WebSockets con Redis Pub/Sub]]
- 🔄 [[04-arquitectura-hibrida-realtime|Arquitectura Híbrida: REST + Eventos Real-time]]

---

## 1️⃣1️⃣ Webhooks, Task Queues & Mensajería 🪝📫

- 🪝 [[01-diseno-webhooks|Diseño y consumo de Webhooks asíncronos]]
- 🔒 [[02-seguridad-webhooks-hmac|Seguridad de Webhooks con firmas HMAC (SHA-256)]]
- 📥 [[03-background-queues-bullmq|Background Queues con BullMQ y Redis]]
- 🔁 [[04-resiliencia-queues-dlq|Resiliencia en Filas: Reintentos, Backoff y DLQ]]
- 📮 [[05-message-brokers-rabbitmq-kafka|Message Brokers: RabbitMQ y Apache Kafka (EDA)]]

---

## 1️⃣2️⃣ Concurrencia Avanzada, Worker Threads & Cluster 🧵⚡

- 🔄 [[01-cluster-module|Escalado vertical con el módulo Cluster y Round-Robin]]
- 🧵 [[02-worker-threads|Worker Threads (node:worker_threads) y SharedArrayBuffer]]
- ⚖️ [[03-cluster-vs-workers-vs-child|Comparativa: Cluster vs Workers vs Child Processes]]
- ☁️ [[04-edge-functions-serverless|Edge Functions y Serverless con Node.js]]

---

## 1️⃣3️⃣ Profiling, Memory Leaks & Performance Tuning 📈🔍

- 🔍 [[01-profiling-cpu-flamegraphs|Profiling de CPU con DevTools e inspección de Flamegraphs]]
- 🧹 [[02-memory-leaks-heapdump|Diagnóstico de Memory Leaks con Heap Snapshots]]
- ⏱️ [[03-metricas-event-loop|Latencia del Event Loop con node:perf_hooks]]
- 🚀 [[04-benchmarking-autocannon-k6|Benchmarking y pruebas de carga con Autocannon y k6]]

---

## 1️⃣4️⃣ Dockerización, Observabilidad & DevOps Pro 🐳🚀

- 🐳 [[01-docker-multi-stage|Docker Multi-Stage Builds e imágenes Distroless]]
- 🛑 [[02-graceful-shutdown|Graceful Shutdown con señales SIGTERM y SIGINT]]
- 📝 [[03-structured-logging-pino|Structured Logging JSON de alto rendimiento con Pino]]
- 📊 [[04-opentelemetry-prometheus|Métricas Prometheus y Trazado con OpenTelemetry]]
- 🚀 [[05-orquestacion-pm2-k8s|Orquestación de procesos con PM2 y Kubernetes]]
