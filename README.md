## Auth Web Microservice with Rust using Actix Web

### Flow of the event would look like this:

- Registers with email address ➡ Receive an 📨 with a link to verify
- Follow the link ➡ register with same email and a password
- Login with email and password ➡ Get verified and receive auth cookie

### Available Routes

- [GET /](http://localhost:8080/)
- [POST /api/invitation](http://localhost:8080/api/invitation)
- [POST /api/register/:invitation_id](http://localhost:8080/api/register/:invitation_id)
- [GET /api/auth](http://localhost:8080/api/auth)
- [POST /api/auth](http://localhost:8080/api/auth)
- [DELETE /api/auth](http://localhost:8080/api/auth)

### Crates Used

- [actix-web](https://crates.io/crates/actix-web) // Actix Web is a simple, pragmatic and extremely fast web framework for Rust.
- [rust-argon2](https://crates.io/crates/rust-argon2) // crate for hashing passwords using the cryptographically-secure Argon2 hashing algorithm.
- [chrono](https://crates.io/crates/chrono) // Date and time library for Rust.
- [diesel](https://crates.io/crates/diesel) // A safe, extensible ORM and Query Builder for PostgreSQL, SQLite, and MySQL.
- [dotenv](https://crates.io/crates/dotenv) // A dotenv implementation for Rust.
- [derive_more](https://crates.io/crates/derive_more) // Convenience macros to derive traits easily
- [env_logger](https://crates.io/crates/env_logger) // A logging implementation for log which is configured via an environment variable.
- [futures](https://crates.io/crates/futures) // An implementation of futures and streams featuring zero allocations, composability, and iterator-like interfaces.
- [lazy_static](https://docs.rs/lazy_static) // A macro for declaring lazily evaluated statics.
- [r2d2](https://crates.io/crates/r2d2) // A generic connection pool.
- [serde](https://crates.io/crates/serde) // A generic serialization/deserialization framework.
- [serde_json](https://crates.io/crates/serde_json) // A JSON serialization file format.
- [serde_derive](https://crates.io/crates/serde_derive) // Macros 1.1 implementation of #[derive(Serialize, Deserialize)].
- [sparkpost](https://crates.io/crates/sparkpost) // Rust bindings for sparkpost email api v1.
- [uuid](https://crates.io/crates/uuid) // A library to generate and parse UUIDs.

Read the full tutorial series on [gill.net.in](https://gill.net.in)

- [Auth Web Microservice with Rust using Actix Web v2 - Complete Tutorial](https://gill.net.in/posts/auth-microservice-rust-actix-web1.0-diesel-complete-tutorial/)

### Dependencies

On Ubuntu 19.10:

```
sudo apt install libclang-dev libpq-dev
```

### Directions For Serving The Static Site 

1. `npm install -g reload` 
2. `cd static`
3. `reload -p 3000 -b`
