# Changelog

All notable changes to Aniverse are documented here.

---

## [1.3] — 2026-07-27

### Fixed
- White blank screen on player page — player now loads correctly every time
- Various UI/UX inconsistencies resolved across home, player, and detail pages

### Added
- **3D Hero Banner** — redesigned home carousel with depth layers and glass-morphism
- **Media Card Expand** — long-press any card to expand with title, synopsis, score, and quick-action buttons (Info · Share · Play · Watchlist)
- **Swipe Up to Play** — on expanded hero/card, swipe up to jump straight into playback
- **Embed + Aniverse Player selection** — Available Providers section on player page; choose Embed, Dub, or language-specific streams (English-S1, English-S3, etc.)
- **Manga Swipe Mode** — page-by-page horizontal swipe in addition to scroll; toggle in reader settings
- **Continue Reading** — manga chapter + exact page saved; resume from home Continue Reading row
- **Full Theme System** — System / Dark / Light modes with 6 accent presets: Sky · Mono · Aqua · Violet · Rose · Lime
- **Custom Accent Colours** — pick any Main + Soft colour pair; unlocks after 30-day watch streak
- **Rounded Corners + Glass Strength** — sliders with live preview
- **Refresh Rate Control** — manual lock at 60 / 90 / 120 Hz or Auto
- **Profile & Watch Stats** — Day Streak · Episodes · Watch Time · Best Streak on profile page
- **Watchlist Tabs** — filter by All · Anime · Movies · Manga

---

## [1.1] — 2025-07-26

### Fixed
- Episode image fallback: TMDB grid cards now show a dim cover/banner when `still_path` is missing
- AniList resolution no longer gets stuck in loading state
- Player control fade animations corrected

### Added
- TMDB / AniList source toggle in episodes header
- Arc-based episode navigation (arc pills ≤100 eps, dropdown >100 eps)
- Desktop prev/next episode arrows (≥768px)
- `anilistResolver` filters TV vs MOVIE results

---

## [1.0.0] — Initial Release

### Added
- Multi-audio playback (Hindi, Tamil, Malayalam, English, Japanese)
- Auto skip intro & outro · Auto Next episode
- Server 1 & Server 2 support
- TMDB + AniList episode integration
- Filler episode markers
- Dark themed UI


### Fixed
- Episode image fallback: TMDB grid cards now show a dim cover/banner when `still_path` is missing — no more blank dark cards
- AniList resolution no longer gets stuck in loading state
- Player control fade animations corrected

### Added
- **TMDB / AniList source toggle** in episodes header (anime only, shown when AniList `streamingEpisodes` data is available)
  - TMDB mode: existing season row + range dropdown behaviour
  - AniList mode: arc pills (horizontal scroll) for ≤100 eps, dropdown for >100 eps; uses AniList thumbnails & titles
- **Arc-based episode navigation** — arc names parsed from AniList episode title format
- **Desktop prev/next episode arrows** — floating buttons on left/right of player, hidden on mobile (flex at ≥768px)
- `anilistResolver` now filters title-search results by format (TV vs MOVIE) to avoid wrong matches

---

## [1.0.0] — Initial Release

### Added
- Multi-audio playback (Hindi, Tamil, Malayalam, English, Japanese)
- Auto skip intro & outro
- Server 1 & Server 2 support
- TMDB + AniList episode integration
- Arc-based episode navigation with arc pills
- Episode range dropdown for 100+ episode seasons
- TMDB / AniList source toggle for episode thumbnails & titles
- Filler episode markers
- Desktop prev/next episode arrows
- Dark themed UI
