# Postiz Improved — Fork Doctor Analysis

**Source:** gitroomhq/postiz-app (29K ⭐)
**Fork:** c6zks4gssn-droid/postiz-improved
**License:** AGPL-3.0

## Platform Support (35!)
Bluesky, Dev.to, Discord, Dribbble, Facebook, Farcaster, GMB, Hashnode, Instagram, Kick, Lemmy, LinkedIn, Listmonk, Mastodon, Medium, MeWe, Moltbook, Nostr, Pinterest, Reddit, Skool, Slack, Telegram, Threads, TikTok, Twitch, VK, Whop, WordPress, X, YouTube

## Planned Improvements (Bonanza Labs)

### 1. 🔐 Agent Wallet Integration
- Add `bonanza-wallet` payment layer for AI agent posts
- Policy-based approval: auto-approve under $X, human approval above
- Multi-chain: Solana, Base, BSC (USDC/USDT/USD1)

### 2. 🤖 Bonanza Agents Integration
- Replace basic agent CLI with Bonanza Agents orchestration
- Multi-step workflows: search → script → post → analyze
- Tool chaining with 6 built-in tools

### 3. 📡 Bonanza Webhooks
- Incoming webhooks for auto-posting triggers
- GitHub push → auto-announce on all platforms
- Price alerts → auto-post to Telegram/Discord

### 4. 📊 Bonanza Analytics
- Replace basic analytics with privacy-first Bonanza Analytics
- AI-powered insights (via Bonanza Agents)
- No cookies, no PII

### 5. 🎬 FrameForge Video Generation
- Auto-generate videos from posts
- HeyGen avatar integration for news posts
- Multiple formats: 16:9, 9:16, 1:1

### 6. 🔍 Bonanza Search
- Auto-research content before posting
- Fact-check with web search
- Trend analysis

### 7. 🩺 Fork Doctor CI/CD
- Add GitHub Actions with Fork Doctor checks
- SBOM generation
- Dev Container support
- Security scanning

### 8. 🐳 Docker Improvements
- Multi-stage builds for smaller images
- Health checks
- Non-root user
- Resource limits

### 9. 📱 Better CLI
- `postiz schedule "tweet" --platforms x,linkedin,threads --time "9am"`
- `postiz agent run --topic "AI news" --style viral`
- `postiz analytics --period 7d --platform x`

### 10. 🔑 Bonanza Auth
- Agent API keys (bza_ prefix) for programmatic access
- JWT tokens for multi-user agencies
- Scope-based permissions per platform

## Architecture
- **Monorepo:** pnpm workspace
- **Backend:** NestJS
- **Frontend:** Vite + React
- **Orchestrator:** Temporal (background jobs)
- **Agent:** LangGraph-based graph service
- **Database:** PostgreSQL (Prisma ORM)

## Key Files
- `apps/backend` — API server
- `apps/frontend` — React UI
- `apps/orchestrator` — Temporal workflows
- `apps/commands` — CLI commands
- `libraries/nestjs-libraries` — shared services
- `libraries/react-shared-libraries` — shared React components