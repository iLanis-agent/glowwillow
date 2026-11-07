# Glowwillow 1.0 TEST

Native Android Hotaru Beam network puzzle. Android 8+ (min26), target35. Package com.gg007.glowwillow.

## Rules
Tap between two neighboring grid points to toggle a beam segment. Every gold dot on a white circle starts exactly one beam. A beam follows grid edges and ends at a plain side of a circle, possibly its own circle. It may not end at a gold dot, pass through a circle, cross, branch or revisit a non-circle grid point. The digit in its starting circle gives the exact number of right-angle turns before reaching the ending circle. Zero means straight. Circle junctions do not add turns to the beams ending or starting there. All circles and beams must form ONE connected network. Branching and joining are allowed only at circles. Unused grid points and edges may remain. Twelve unique 3x3-point circle/direction/count boards with twelve distinct solutions, undo/reset/next/level selection and saved glow palette/edge-guide settings.

## Download and status
https://mega.co.nz/#!UFdBVBoD!H4ef-Cw07NuXzAZB_ygUWCIE-hP4t8QmHhm7B9VErC4
APK SHA256 64af5b982b80362d442f309b848c64692a71b0aaa6af6ef89d4efa6370ecf3f6; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

Independent Java simple-path DFS from each circle, disjoint path packing and disjoint-set circle connectivity agree with production degree checks, edge tracing, bend counters and connectivity on ALL 4096 edge masks per board, 49152 total. Each board has exactly one solution. Bounds, invalid masks, solved-input lock, solve, undo and replay pass. Actual archived generator regeneration and archived Java tests pass. Drawing-adapter navigation, saved settings, privacy, edge taps, completion marks, next and level selection pass. Actual game/menu/settings/privacy/levels/solved drawing pixels inspected, not phone screenshots. Phone runtime, performance and external browser handoff QA remain incomplete. Signed TEST only, not final and not Play published.

## Functional difference
Live 803-entry registry, 116 recovered partial README records and semantic review of all 142 cards in the exact Snakefern cumulative stage found no Hotaru Beam match. Prism Relay rotates mirrors for a single optical route through ordered relays; Glowwillow toggles separate grid-edge paths from marked circles into a connected network, with per-path bend counts and circle-only junctions. RuneBriar and Signalfern require one unbranched loop and measure segment lengths; Glowwillow permits branching at circles, unused points, directed source dots, return-to-self beams and per-beam turns. All twelve generated solutions include a branching circle. Known Hotaru Beam genre, not a global invention. Corpus is partial. Rules verified at https://www.nikoli.co.jp/ja/puzzles/hotaru_beam/ and https://www.janko.at/Raetsel/Hotaru-Beam/index.htm .

## Build
JDK17 and Android SDK platform35/build-tools35.0.0. Run python generate-levels.py to reproduce levels.json. Board.java embeds the generated circles, directions, bend counts and solutions. javac -d /tmp/glow-test src/com/gg007/glowwillow/Board.java BoardTest.java and java -cp /tmp/glow-test com.gg007.glowwillow.BoardTest. bash build.sh builds an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not a final store release.

## Privacy and branding
Glowwillow runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Glow palette, edge guides and completed-puzzle marks stay in the app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon copied byte-for-byte from preserved original. Menu includes studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation
Complete source and APK privately preserved at https://files.instinct.com/bzk5t6gyfew4-glowwillow-source-archive with exact cumulative staged HTML. GitHub https://github.com/iLanis-agent/glowwillow holds README only; full Git source commit remains pending. Cumulative stage is NOT LIVE; existing studio run remains queued. No Pages settings changes, rollback or Play rollout. Updated November 7, 2026.
