# IPTV playlists

Small collection of M3U playlists focused on Portuguese TV and radio streams.

## Files

- `oloco.m3u` — curated playlist with Portuguese TV/radio entries and custom category adjustments.
- `teste.m3u` — alternate/test playlist kept separately from the main curated file.

## Format

The playlists use the extended M3U format (`#EXTM3U` / `#EXTINF`). Some entries also include player-specific metadata such as `#EXTVLCOPT` or `#KODIPROP`.

`oloco.m3u` references external EPG sources in its header so compatible players can display programme-guide information when those sources are available.

## Usage

Open one of the `.m3u` files with an IPTV-compatible player such as VLC or Kodi, or import the raw playlist URL into a compatible client.

Stream availability depends on the upstream providers. A playlist entry can stop working even when the file itself has not changed.

## Repository scope

This repository stores playlist metadata and stream references; it does not host the video or radio streams themselves.

The main playlist is based on public/official stream references and includes local categorisation adjustments. Always respect the terms and geographic restrictions of the upstream providers.

## Maintenance notes

When updating a playlist:

- keep the `#EXTM3U` header intact;
- preserve `tvg-id`, logos and group titles unless there is a verified reason to change them;
- avoid committing credentials, private tokens or personal playlist URLs;
- prefer small, reviewable changes so broken entries are easy to identify.
