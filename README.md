## Hi, I'm Aashwin 👋

MTech in Information Systems Security at **NIT Jamshedpur** (2025–27). I build backend-heavy
full-stack systems and I care about correctness under failure: races, retries and
bad data.

### Featured projects

**[IoT Fleet Monitor](https://github.com/Aash55/iot-fleet-monitor)** · [live demo](https://iot-fleet-monitor.vercel.app)
Demo login: `ash@fleet.local` / `fleetmon123` · devices show live data only while the simulator runs (see screenshots in the repo)
Telemetry pipeline with ML intrusion detection and prevention.
Express → Redis Streams → consumer → PostgreSQL, scored in-process by a Random Forest exported to ONNX.
- Trained on CICIoT2023 (46.7M rows, 33 attack types); found and removed a data leak that gave a fake F1 of 0.991
- Alert threshold at 0.40% false positives: macro recall 0.721 on a held-out test set used once
- Node ONNX output matches scikit-learn on all 57,464 test rows (max difference 6.1e-7)

**[SnapSeat](https://github.com/Aash55/SnapSeat)** · [live demo](https://snapseat-web.onrender.com)
Demo login: `user1@test.com` / `password123` · organizer: `organizer@snapseat.com`
Event ticketing with atomic seat holds and idempotent payments.
- Double-booking and double-charging are prevented by database constraints and row locks, not only app code
- 27 tests against real PostgreSQL, including 10 users racing for one seat and 5 identical payments sent at once
- HMAC-signed, timestamped webhooks with duplicate-delivery protection

### Tech I've used in these projects
**Languages:** JavaScript, Python, SQL, C++
**Backend:** Node.js, Express, PostgreSQL, Redis Streams, Sequelize, JWT, argon2
**Frontend:** React, Vite, TanStack Query, Tailwind CSS, Recharts
**ML:** scikit-learn, pandas, ONNX Runtime
**Deploy:** Render, Vercel, Neon, Upstash

### Also
- GATE CS 2025: AIR 8,799 of 1.7 lakh candidates
- First-author research paper on continuous authentication (BehavCont), submission in progress
- Currently: DSA (Striver A2Z) and system design

📫 [LinkedIn](https://www.linkedin.com/in/aashwin-upadhyay) · 2025pgcsis11@nitjsr.ac.in
