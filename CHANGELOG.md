# Changelog

All notable changes to Aniverse are documented here.

---

## [1.1.8] — 2026-08-03

### Added
- **Download for All Streams** — download any episode from Direct, Dubbed, Language streams or Native HLS; runs in background with progress indicator; accessible from Library for offline playback
- **Details Page Overhaul** — studios, aired date, episode duration, source type (manga/LN/original); related anime cards (sequels, prequels, side stories); inline trailer embed; skeleton loading

### Improved
- **Animations** — spring-based physics throughout; hero banner swipes, episode card reveals, provider panel, and page transitions all reworked for a more native feel
- **Library tab** — downloaded episodes listed with progress, file size, and quick-play button

---

## [1.1.7] — 2026-08-01

### Added
- **AI Caption Translation** — online subtitles can now be auto-translated to your preferred language using Claude AI; works with Jimaku, OpenSubtitles, and Wyzie sources
- **Random Suggestion** — new shuffle button on the home screen drops you into a random highly-rated anime pick, perfect for when you can't decide what to watch
- **Manga UI Overhaul** — cleaner reader layout with edge-to-edge pages, gesture-based zoom, and per-chapter quick-jump from the TOC overlay
- **Manga Reading Made Easier** — tap-to-seek within a chapter, pinch-to-zoom on any panel, and persistent last-read position synced across sessions
- **Season Tabs in Player** — multi-season anime (Demon Slayer, AOT, JJK, etc.) now show Season 1 / Season 2 / … tabs above the episode list for instant navigation between seasons

### Improved
- **Player UI refresh** — updated server/source panel with provider logos, cleaner autoplay countdown card, and smoother fullscreen landscape lock
- **Details page** — AniList resolution now shows disambiguation cards when multiple matches found; never silently fails
- **Browse page** — TV channel and OTT platform chips now show logos instead of text; results display as Top-10-style list rows with backdrop
- **Subtitle panel** — filenames shown as primary label; English subtitles sorted first; single-select fixed (no more all-ON bug)
- **Profile** — streak-based reward milestones show exact days remaining to next unlock; animated flame in profile card banner

### Fixed
- Videasy domain updated from `.net` → `.to`; player loads correctly again
- Season resolution no longer shows 60+ flat episodes for multi-season anime
- Subtitle providers (OpenSubtitles, Wyzie, Podnapisi) now correctly receive IMDB ID via AniList `externalLinks` — all providers load, not just Jimaku
- Community page avatar frames and animated gradient usernames now render correctly
- Watch button on details page never silently fails — always navigates even if AniList resolution times out

---

## [1.1.6] — 2026-07-31

### Fixed
- Replaced the oversized double-tap seek effect with compact, smooth feedback
- Removed the blue full-volume highlight for consistent player styling
- Protected bright scenes from washed-out enhancement and excessive contrast

### Improved
- Added restrained colour smoothing while preserving anime line detail
- Refined CinePlayer enhancement levels for cleaner playback

---

## [1.1.5] — 2026-07-31

### Fixed
- Player video remains visible when the CinePlayer controls fade out
- Improved subtitle upload and online caption handling
- Corrected player sizing and episode information on different Android displays
- Refined playback server fallback and stream-loading behavior

### Added
- In-app update checks and direct APK update flow
- Downloaded and offline playback improvements
- Playback language, quality, and subtitle preferences
- Expanded theme and accessibility customization

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
