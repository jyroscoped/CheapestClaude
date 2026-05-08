# CheapestClaude
Claude users do not have a simple, visual way to know when their session burn will be cheapest, especially when peak-hour behavior changes how fast usage gets consumed. Some users are already tracking peak/off-peak windows with extensions because the timing matters enough to change how quickly they run through their quota.

## MVP dashboard

This repository now includes a lightweight single-page web app at:

- `index.html`

### Features

- Usage timeline by timestamp with estimated burn intensity
- Current peak/off-peak indicator
- Hourly cheapest-time chart (relative burn estimate)
- Prompt recommendation (`prompt now`, `wait for cheaper window`, `high burn`)
- Session history summaries by recent day
- CSV import and manual prompt logging (stored in browser localStorage)

### CSV format

Expected header columns:

`timestamp,timezone,session_id,model,estimated_tokens,peak_flag,burn_score`
