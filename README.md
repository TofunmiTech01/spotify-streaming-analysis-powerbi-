# 🎵 Spotify Personal Listening History Dashboard (2013–2024) — Power BI Analytics Project

> **A comprehensive Power BI dashboard analyzing 11+ years of personal Spotify streaming data — 149,860 streams, 5,342 hours of music, 4,113 unique artists, 7,944 albums, and 13,838 tracks — uncovering deep behavioral patterns in music consumption, platform usage, listening habits, and artist loyalty across a decade.**

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [What Makes This Project Unique](#what-makes-this-project-unique)
- [Dataset Summary](#dataset-summary)
- [Tools & Technologies](#tools--technologies)
- [Dashboard Preview](#dashboard-preview)
- [Key Performance Indicators (KPIs)](#key-performance-indicators-kpis)
- [Analytical Insights](#analytical-insights)
  - [11-Year Streaming Journey](#1-11-year-streaming-journey)
  - [Platform Behavior Analysis](#2-platform-behavior-analysis)
  - [Listening Hour & Day Patterns](#3-listening-hour--day-patterns)
  - [Artist Loyalty & Dominance](#4-artist-loyalty--dominance)
  - [Album Deep Dive](#5-album-deep-dive)
  - [Track Obsession Analysis](#6-track-obsession-analysis)
  - [Shuffle & Skip Behavior](#7-shuffle--skip-behavior)
  - [Engagement & Completion Rate](#8-engagement--completion-rate)
  - [Monthly & Seasonal Patterns](#9-monthly--seasonal-patterns)
  - [The Night Owl Phenomenon](#10-the-night-owl-phenomenon)
- [Strategic Insights & Self-Reflections](#strategic-insights--self-reflections)
- [Live Dashboard](#live-dashboard)
- [Connect With Me](#connect-with-me)

---

## Project Overview

Most people know their Spotify Wrapped. This goes far deeper.

This project transforms **11 years of raw personal Spotify streaming history** (2013–2024) into a fully interactive, dual-page Power BI dashboard that answers questions most music analytics never ask: *When exactly do you listen? Are you genuinely engaged or skipping? Do you own the night? Which artists have been with you the longest? How has your music consumption evolved year by year?*

The result is a behavioral self-portrait told through data — covering **149,860 individual stream events**, **5,342 hours of listening**, and a journey across **6 platforms**, **4,113 artists**, and **13,838 unique tracks** from July 2013 to December 2024.

---

## What Makes This Project Unique

Unlike standard business dashboards, this project analyzes **personal behavioral data** — making the insights both technically rigorous and genuinely personal. It demonstrates:

- Ability to work with **real, messy, time-series behavioral data** at scale
- Advanced **Power BI development** including heatmaps, scatter plots with dynamic sliders, YoY comparison cards, and platform-filtered views
- **Behavioral analytics thinking** — going beyond "what was played" to "how, when, and why"
- Full **dual-page dashboard architecture** with consistent Spotify-branded dark theme and interactive cross-filtering

---

## Dataset Summary

| Attribute | Detail |
|---|---|
| **Period Covered** | July 8, 2013 – December 15, 2024 |
| **Total Stream Events** | 149,860 |
| **Total Listening Time** | 320,492 minutes (5,342 hours / 223 days) |
| **Unique Tracks** | 13,838 |
| **Unique Artists** | 4,113 |
| **Unique Albums** | 7,944 |
| **Platforms** | Android, Cast to Device, iOS, Mac, Windows, Web Player |
| **Key Fields** | spotify_track_uri, timestamp, platform, ms_played, track_name, artist_name, album_name, reason_start, reason_end, shuffle, skipped |

---
## Tools & Technologies

- **Power BI Desktop** — Dual-page dashboard design, DAX measures, interactive visuals
- **Power Query (M Language)** — Data transformation, time extraction, behavioral flag engineering
- **DAX** — YoY comparison measures, weekday/weekend splits, dynamic KPI cards, average listening time calculations
- **Microsoft Excel / CSV** — Raw personal data source (Spotify Extended Streaming History export)

---

## Dashboard Preview

**Page 1 — Albums, Artists & Tracks Overview**
![Spotify Dashboard Page 1](https://github.com/TofunmiTech01/spotify-streaming-analysis-powerbi-/blob/main/spotify-dashboard1.jpeg)

**Page 2 — Listening Hours Heatmap & Engagement Analysis**
![Spotify Dashboard Page 2](https://github.com/TofunmiTech01/spotify-streaming-analysis-powerbi-/blob/main/spotify-dashboard2.jpeg)

---

## Key Performance Indicators (KPIs)

| KPI | Value |
|---|---|
| **Total Stream Events** | 149,860 |
| **Total Listening Time** | 5,342 hours (223 full days) |
| **Unique Tracks Played** | 13,838 |
| **Unique Artists Played** | 4,113 |
| **Unique Albums Played** | 7,944 |
| **Avg Listening Time per Stream** | 2.14 minutes |
| **Median Listening Time per Stream** | 2.31 minutes |
| **Primary Platform** | Android (93.3%) |
| **Shuffle Rate** | 74.5% of all streams |
| **Skip Rate** | 5.3% of all streams |
| **Genuine Listens (>30 seconds)** | 62.9% of streams |
| **Late Night Listening (midnight–6am)** | 34.3% of all streams |

### Latest Year Performance (2024 vs 2023):
| Metric | 2024 | 2023 | YoY Change |
|---|---|---|---|
| Albums Played | 1,802 | 2,258 | **-20.19%** |
| Artists Played | 1,058 | 1,400 | **-24.43%** |
| Tracks Played | 3,508 | 3,916 | **-10.42%** |

---

## Analytical Insights

### 1. 11-Year Streaming Journey

The streaming history tells a vivid story of how music consumption evolves across a decade of life:

| Year | Streams | Hours | Unique Artists | Unique Tracks |
|---|---|---|---|---|
| 2013 | 185 | 8 | 63 | 149 |
| 2014 | 23 | 1 | 21 | 23 |
| 2015 | 2,809 | 59 | 610 | 1,357 |
| 2016 | 6,413 | 198 | 458 | 2,535 |
| **2017** | **26,320** | **671** | **647** | **3,326** |
| 2018 | 14,817 | 474 | 439 | 2,917 |
| 2019 | 14,927 | 479 | 493 | 2,934 |
| **2020** | **24,280** | **921** | **820** | **3,928** |
| **2021** | **22,991** | **892** | **1,578** | **5,126** |
| 2022 | 16,202 | 642 | 1,220 | 4,477 |
| 2023 | 11,023 | 515 | 1,456 | 4,042 |
| 2024 | 9,870 | 483 | 1,072 | 3,587 |

**Key Findings:**

- **2014 is the anomaly year** — only 23 streams in an entire year. This almost certainly reflects a gap in Spotify usage (perhaps a different streaming service, or a period away from music platforms entirely) rather than a genuine preference shift.
- **2017 was the peak streaming year** — 26,320 streams and 671 hours. A +310% jump from 2016. Something triggered an explosion in music consumption this year — the data points to deep Beatles, Killers, and John Mayer listening sessions dominating the calendar.
- **2020 was the second peak at 921 hours** — the highest listening *hours* of any year, exceeding even 2017. The pandemic's stay-at-home context almost certainly drove this surge. Music became a primary companion in 2020.
- **2021 marks the Artist Diversity Peak** — 1,578 unique artists explored, the highest of any year. The pandemic-era openness to discovering new music carried into 2021, resulting in the broadest listening portfolio ever recorded.
- **2022–2024 show a consistent declining trend** — streams have fallen from 16,202 (2022) → 11,023 (2023) → 9,870 (2024). This is a 39% decline from 2022 to 2024. Whether driven by competing entertainment (podcasts, video), life changes, or simply listening fatigue, the trend warrants attention.
- **The post-2021 decline is in streams and diversity** — 2023 still explored 1,456 unique artists despite lower streams, suggesting that listening is becoming more selective and intentional rather than background-heavy.

---

### 2. Platform Behavior Analysis

| Platform | Streams | Share | Skip Rate | Shuffle Rate |
|---|---|---|---|---|
| **Android** | 139,821 | **93.3%** | 5.2% | 77.1% |
| Cast to Device | 3,898 | 2.6% | 0.0% | 0.1% |
| iOS | 3,049 | 2.0% | **10.3%** | 69.2% |
| Windows | 1,691 | 1.1% | **14.1%** | 59.6% |
| Mac | 1,176 | 0.8% | 6.1% | 54.3% |
| Web Player | 225 | 0.2% | 0.0% | 0.0% |

**Key Findings:**

- **Android is the overwhelming primary platform at 93.3% of all streams** — this is not a casual preference; it is the near-exclusive listening environment. The smartphone is the music player, full stop.
- **Cast to Device and Web Player have 0% skip rates** — when casting to a speaker or using the web player, there is zero skipping behavior. These are intentional, deliberate listening sessions — likely social or ambient music settings where the listener commits to the queue.
- **Windows has the highest skip rate at 14.1%** — desktop listening is exploratory and impatient. When at a computer, there's a tendency to browse through tracks rather than settle into them. The skip rate is nearly 3x the Android rate.
- **iOS skip rate (10.3%) is double Android's (5.2%)** — despite both being mobile platforms, iOS sessions are more skip-heavy, possibly reflecting different usage contexts (commuting vs. home relaxing).
- **Android's 77.1% shuffle rate vs. Mac's 54.3%** reveals that mobile listening is predominantly shuffle-mode while desktop/laptop listening is more intentional with curated playlists or album listening.

---

### 3. Listening Hour & Day Patterns

#### Hourly Distribution (Total Streams):

| Time Block | Hours | Total Streams | Character |
|---|---|---|---|
| **Midnight–3am** | 0–3 | 37,858 | 🌙 Peak Night Zone |
| Early Morning | 4–6 | 20,888 | Night trailing off |
| Morning | 7–11 | 10,531 | Sharp daytime drop |
| Midday | 12–13 | 2,382 | Absolute low |
| Afternoon | 14–16 | 8,241 | Gradual recovery |
| **Evening** | 17–19 | 26,304 | 📈 Evening surge |
| **Late Night** | 20–23 | 38,678 | 🔥 Second peak |

**Peak hours:** Midnight (10,884), 11pm (10,516), 8pm (10,494), 1am (9,395), 5pm (9,194)
**Lowest hour:** Noon (724 streams)

#### Day of Week:

| Day | Streams | Share |
|---|---|---|
| **Friday** | 25,646 | **17.1%** |
| **Wednesday** | 23,406 | 15.6% |
| Thursday | 21,401 | 14.3% |
| Monday | 21,031 | 14.0% |
| Tuesday | 20,705 | 13.8% |
| Saturday | 19,397 | 12.9% |
| **Sunday** | 18,274 | **12.2%** (lowest) |

**Key Findings:**

- **The listening pattern reveals a strong nocturnal identity.** The two peak listening windows are midnight–3am and 8pm–midnight. Combined, these four hours account for a disproportionate share of total listening — music is fundamentally a night-time activity.
- **Noon is the dead zone** — only 724 streams in the entire dataset occur at 12pm. The lunch hour is essentially silent. This could reflect work/school commitments or simply that midday is not a music-oriented time.
- **The 7am–1pm block shows the sharpest activity drop** — from 4,412 streams at 7am to just 724 at noon — an 84% decline in 5 hours. Morning hours involve real-world engagement that crowds out passive music listening.
- **Friday is the biggest music day** at 25,646 streams — the anticipation of the weekend, end-of-week mood, and increased social/leisure time converge on Friday to create peak listening conditions.
- **Sunday is the quietest day** at 18,274 streams — counter-intuitively, the most "relaxed" day of the week generates the least music. Sunday listening may shift to podcasts, silence, or outdoor activity.
- **Weekdays (112,189 streams) generate 74.8% of total streams** vs weekends (37,671 / 25.2%) — music is a weekday companion, not primarily a weekend leisure activity.

---

### 4. Artist Loyalty & Dominance

#### Top 10 Artists by Total Streams (All-Time):

| Rank | Artist | Streams | Listening Hours |
|---|---|---|---|
| 1 | **The Beatles** | 13,621 | **336 hours** |
| 2 | The Killers | 6,878 | 294 hours |
| 3 | John Mayer | 4,855 | 201 hours |
| 4 | Bob Dylan | 3,814 | 158 hours |
| 5 | Paul McCartney | 2,697 | 99 hours |
| 6 | Led Zeppelin | 2,482 | 69 hours |
| 7 | Johnny Cash | 2,478 | 67 hours |
| 8 | The Rolling Stones | 2,390 | 86 hours |
| 9 | Radiohead | 2,305 | 60 hours |
| 10 | The Black Keys | 2,231 | 53 hours |

**Key Findings:**

- **The Beatles at 13,621 streams is not just the #1 artist — it is in a completely different category.** The #2 artist (The Killers at 6,878) has barely half the streams. The Beatles represent 9.1% of all streams in the entire dataset — nearly 1 in every 10 songs played across 11 years was a Beatles track. This is extraordinary single-artist loyalty.
- **The top 10 artists are dominated by classic rock and Americana** — Beatles, Dylan, Zeppelin, Cash, Rolling Stones, Paul McCartney. The listening identity is deeply rooted in the musical canon of the 1960s–1980s.
- **The Killers (6,878) and John Mayer (4,855) are the modern-era representatives** in an otherwise classic-dominated top 10 — suggesting a musical identity that bridges timeless classics with contemporary rock/alternative.
- **The 2021 artist diversity peak (1,578 unique artists)** stands in stark contrast to the top-artist concentration — showing the ability to both obsessively deep-dive into favorites AND broadly explore new territory simultaneously.
- **In 2017 (the peak year), The Beatles had 3,244 streams** — nearly 25% of all 2017 listening was Beatles. A clear year of intensive artist deep-diving.

---

### 5. Album Deep Dive

#### Top 10 Albums by Total Streams:

| Rank | Album | Artist | Streams |
|---|---|---|---|
| 1 | **The Beatles** (White Album) | The Beatles | 2,063 |
| 2 | Past Masters | The Beatles | 1,672 |
| 3 | Abbey Road | The Beatles | 1,429 |
| 4 | The Wall | Pink Floyd | 1,241 |
| 5 | Revolver | The Beatles | 1,038 |
| 6 | Help! | The Beatles | 979 |
| 7 | At Folsom Prison | Johnny Cash | 918 |
| 8 | Sgt. Pepper's Lonely Hearts Club Band | The Beatles | 910 |
| 9 | Exile On Main Street | The Rolling Stones | 892 |
| 10 | Hot Fuss | The Killers | 878 |

**Key Findings:**

- **5 of the top 10 albums are by The Beatles** — confirming that the Beatles obsession is not just about singles or shuffled tracks, but deep, album-oriented listening. The Beatles' entire catalogue has been consumed extensively and repeatedly.
- **The White Album (2,063 streams) is the most-played album in the entire 11-year history** — a double album of 30 tracks, suggesting it has been returned to again and again across years, not just binged once.
- **Abbey Road, Revolver, Help!, and Sgt. Pepper's** all feature independently — four of the most critically acclaimed albums in history, all in personal top 10. This reflects genuine musical depth, not algorithmic recommendation consumption.
- **The Wall (Pink Floyd) at #4** is the highest non-Beatles album — a conceptual rock masterpiece that requires active, attentive listening. Its presence at #4 further confirms the listening identity leans toward albums as experiences, not just songs as background.
- **At Folsom Prison (Johnny Cash) at #7** is the outlier — a live album from 1968 that continues to captivate decades after release. Johnny Cash's presence in both the album and artist top 10 points to a genuine Americana and storytelling thread running through the musical identity.

---

### 6. Track Obsession Analysis

#### Top 10 Most-Played Tracks (All-Time):

| Rank | Track | Streams |
|---|---|---|
| 1 | **Ode To The Mets** (The Strokes) | 207 |
| 2 | In the Blood (John Mayer) | 181 |
| 3 | Dying Breed (The Killers) | 166 |
| 4 | Caution (The Killers) | 164 |
| 5 | 19 Dias y 500 Noches — En Directo | 148 |
| 6 | For What It's Worth (Buffalo Springfield) | 146 |
| 7 | Concerning Hobbits (Howard Shore) | 142 |
| 8 | All These Things That I've Done (The Killers) | 142 |
| 9 | Come Together — Remastered 2009 (The Beatles) | 137 |
| 10 | The Boxer (Simon & Garfunkel) | 135 |

**Key Findings:**

- **"Ode To The Mets" by The Strokes tops the all-time chart at 207 plays** — a deeply nostalgic, cinematic track that clearly resonates on a personal level far beyond casual listening. Playing any song 207 times across 11 years is a statement of emotional attachment.
- **John Mayer's "In the Blood" at 181 plays** is a deeply introspective track about family patterns and self-identity — its personal resonance likely drives the repeat listening rather than just musical preference.
- **The Killers place two tracks in the top 10** (Dying Breed + All These Things That I've Done), confirming their status as the dominant modern-era artist in the listening history.
- **"Concerning Hobbits" at #7 (142 plays)** — a Lord of the Rings soundtrack piece — is the most unexpected top-10 entry. Its presence points to use as focus/ambient music during work or study sessions.
- **"The Boxer" by Simon & Garfunkel at #10** rounds out a top-10 that spans six decades of music history — from a 1969 folk classic to a 2020 indie-rock closer. The range of emotional and era diversity in the top tracks is remarkable.
- **The gap between #1 (207) and #10 (135)** is relatively tight — suggesting no single track is astronomically over-played; rather, there is a cluster of deeply loved songs played at consistently high frequencies.

---

### 7. Shuffle & Skip Behavior

| Behavior | Count | Rate |
|---|---|---|
| **Shuffled streams** | 111,583 | **74.5%** |
| **Skipped streams** | 7,869 | **5.3%** |
| Non-shuffled streams | 38,277 | 25.5% |
| Completed streams | 77,194 | 51.5% |
| Forward-button ended | 53,470 | 35.7% |

**Listening Start Reasons:**
- Track done (autoplay): 51.2% — passive, continuous listening
- Forward button: 35.9% — active navigation
- Click/row select: 7.5% — intentional selection

**Key Findings:**

- **74.5% of all streams are shuffled** — the default listening mode is serendipitous rather than curated. Music is consumed as a discovery experience, not a planned sequence.
- **The 5.3% skip rate is remarkably low** — for a 74.5% shuffle rate, one would expect more skipping when the algorithm serves unexpected tracks. The low skip rate suggests either the shuffle algorithm serves well-matched content OR that there is high tolerance and openness to whatever plays next.
- **51.2% of streams start because the previous track ended naturally** — passive, uninterrupted listening is the dominant mode. More than half of all streams begin without any active intervention.
- **The "trackdone" completion rate of 51.5%** confirms that when a song begins, there is a better than 50-50 chance it plays fully — a solid engagement signal for 149,860 total streams.
- **Cast to Device and Web Player have 0% skip rates** — when the music is playing through speakers or in a browser, there is zero skipping. These are the most "committed" listening contexts.

---

### 8. Engagement & Completion Rate

| Engagement Level | Streams | Share |
|---|---|---|
| **Genuine listens (>30 seconds)** | 94,200 | **62.9%** |
| Short plays (<30 seconds) | 55,660 | **37.1%** |

**Key Findings:**

- **37.1% of all streams last under 30 seconds** — more than one in three "plays" is essentially a skip or a browse. This is extremely common in shuffle-heavy listening and reflects the nature of modern streaming: music is sampled, not just consumed.
- **62.9% genuine engagement rate** across 149,860 streams means approximately 94,200 songs were meaningfully listened to — equivalent to listening genuinely to a song every 3.4 minutes for 223 full days.
- The **average stream duration of 2.14 minutes** (vs typical song length of ~3.5 minutes) confirms that many streams are partial listens — but the **median of 2.31 minutes** is slightly higher, suggesting the distribution is influenced by a minority of very-short accidental or immediate skips.
- The scatter plot on Page 2 of the dashboard visualizes **Average Listening Time vs. Track Frequency** — with dynamic sliders allowing filtering to identify the specific tracks that are both frequently played AND fully listened to. These are the true "core favorites" of the listening identity.

---

### 9. Monthly & Seasonal Patterns

| Month | Streams | Character |
|---|---|---|
| January | 12,525 | New year high |
| February | 8,465 | Lowest month |
| March | 9,378 | — |
| April | 12,204 | Spring surge |
| May | 10,068 | — |
| June | 10,680 | — |
| July | 11,619 | Summer rise |
| **August** | **15,737** | 📈 Peak month |
| **September** | **17,733** | 🔥 Highest month |
| **October** | **16,388** | Sustained high |
| November | 13,230 | — |
| December | 11,833 | — |

**Key Findings:**

- **September is the single most active listening month** across the entire 11-year history with 17,733 streams — the transition from summer to autumn appears to be the most music-intensive period of the year.
- **August–October form a listening "Super Season"** — three consecutive months of above-average intensity (15,737 + 17,733 + 16,388 = 49,858 streams = 33.3% of all streams in just 3 months).
- **February is the quietest month** at 8,465 streams — the shortest month with cold weather and post-January energy dip produces the least musical engagement. February is 52% less active than September.
- **The single most active month ever recorded** was September 2017 with 5,176 streams — a single month where, on average, 172 songs were played every day. This was the absolute zenith of music consumption.
- The **July 2017 (3,915)** and **August 2017 (3,191)** also rank in the all-time top 5 months — the summer-autumn 2017 period was an era of extraordinary musical immersion.

---

### 10. The Night Owl Phenomenon

| Time Period | Streams | Share of Total |
|---|---|---|
| **Late night (midnight–6am)** | **51,377** | **34.3%** |
| Evening (6pm–midnight) | 49,278 | 32.9% |
| Daytime (6am–6pm) | 49,205 | 32.8% |

**Key Findings:**

- **34.3% of all listening — over 51,000 streams — happens between midnight and 6am.** This is not occasional late-night listening. This is a structurally nocturnal music habit that has persisted across 11 years of data.
- The **midnight hour (10,884 streams) is the single busiest hour** in the entire dataset — more music is played at midnight than at any other point in the 24-hour cycle. Music consumption peaks precisely when most people are asleep.
- **The daytime dead zone (9am–1pm) accumulates only ~5,500 streams total** — about half what the midnight hour generates alone. The contrast between the busiest and quietest hours is stark.
- **1,714 hours of music were consumed between midnight and 6am** — equivalent to 71 full days of continuous midnight listening across the dataset's lifetime.
- This nocturnal pattern holds remarkably consistent across all platforms and years — it is a deeply ingrained behavioral signature, not a phase or artifact of any particular period.

---

## Strategic Insights & Self-Reflections

### 🎸 The Classic Rock Identity
The top artists (Beatles, Dylan, Zeppelin, Cash, Rolling Stones), top albums (Abbey Road, The Wall, Exile on Main St.), and top tracks (The Boxer, Come Together, For What It's Worth) paint an unmistakable portrait: this is a listener with a deep, genuine love for the musical canon of the 1960s–1970s. Not nostalgia — authentic appreciation.

### 📱 Mobile-First, Nocturnal, Shuffle-Driven
93.3% Android, 34.3% late-night, 74.5% shuffled. The listening profile is a smartphone-in-hand, night-owl, serendipity-seeker who lets music flow rather than controlling every track — but still skips rarely, suggesting genuine openness to what plays.

### 📉 The Post-2021 Fade — A Question Worth Asking
Streams have declined 43% from 2021 to 2024. This deserves honest reflection: is it competing entertainment (video content, podcasts)? Life stage changes reducing idle listening time? Or genuine musical disengagement? The data cannot answer — but it raises the question clearly.

### 🎯 Obsession vs. Exploration — Living Both
The same dataset contains 13,621 Beatles streams (obsession) AND 4,113 unique artists explored (diversity). This is not contradiction — it is a rich musical identity that can go both 100 miles deep on one artist and 100 miles wide across genres simultaneously.

### 🌙 Sleep and Music Are Competing — Music is Winning
51,377 streams after midnight means music is consistently prioritized over sleep. The data doesn't judge — but it notices.

---

## Live Dashboard

> 🔗 Interact with the full live Power BI dashboard **[HERE](#)** *(insert your Power BI app link)*

---

## Connect With Me

Let's connect, collaborate, or talk data!

- 💼 [LinkedIn](https://www.linkedin.com/in/oluwatofunmi-isholadaniel/)
- 💻 [GitHub](https://github.com/TofunmiTech01)

---

*Built with Power BI · Analyzed with precision · Designed for decisions — and a little self-discovery.*
