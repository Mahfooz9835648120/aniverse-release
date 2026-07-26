# Changelog

All notable changes to Aniverse are documented here.

---

## [1.1] — 2025-07-26

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
