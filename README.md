# @encoding/serde_json — JSON Serialization for Zeta

Auto-converted from [serde_json](https://crates.io/crates/serde_json) v1.0.149 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- **to_string / from_str** — serialize/deserialize any `Serialize`/`Deserialize` type to/from JSON
- **Value enum** — dynamic JSON values: Null, Bool, Number, String, Array, Object
- **Streaming** — deserialize from `Read` streams, serialize to `Write` streams
- **Pretty printing** — `to_string_pretty` with configurable indentation
- **Raw values** — `RawValue` for deferred JSON parsing
- **Number handling** — arbitrary precision, `serde_json::Number` type

## Usage
```zeta
use @encoding/serde_json::{self, Value};

let data: Value = serde_json::from_str(r#"{"name":"Zeta","version":1}"#).unwrap();
println!("{}", data["name"]);
```

## Stats: ~7,667 lines, 0 unsupported items

## License: MIT