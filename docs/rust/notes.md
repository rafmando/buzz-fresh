axum - rust web framework
tokio - async runtime
serde - serialization
serde_json
sqlx - database
uuid - unique identifiers
chrono - dates and times
reqwest - http client (for Stytch)
jsonwebtoken - jwt verification     
dotenvy - environment variables 
thiserror - error handling
anyhow - error handling
tacing - logging
tracing-subscriber - logging
tower - tower middleware
tower-http 


Tokio - the async runtime. This is what lets your server handle simtaneous requests without getting blocked.

Axum -  the web framework sitting on top of Tokio. It handles routing — matching incoming URLs to your handler functions.

Cors - you added CorsLayer::permissive() which means your Next.js frontend will be allowed to talk to this backend. Without that the browser blocks cross-origin requests.

Tracing -structured logging. Every request that hits your server gets logged with timing, method, path. Essential for debugging in production.