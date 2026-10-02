# REBOUND · 深渊回响

A real-time ricochet roguelite built with Godot. Aim into advancing enemy formations, move into returning balls, and combine upgrades across three 3D routes.

[Project page & Windows downloads](https://rebound-game.dio-world.chatgpt.site) · [Changelog](#changelog) · [简体中文](#简体中文)

## Repository status

**This repository currently contains this README only. Source code, models, other assets, and build files are not uploaded here.**

- **Latest public game build: v0.36 · A Clearer Wall-Contact Accent**, first published on 2026-10-02 at 19:07:02.024 UTC
- A modest wall-ricochet accent, retaining v0.35's sixteen skill/fusion icons, numeric labels, and compact projectile effects
- The project page has a new charcoal, ivory, and coral design across downloads, updates, screenshots, and feedback
- Downloadable builds, gameplay footage, and screenshots are available on the project page above
- This is a desktop-game project, not a browser-playable game

## The game

- Two playable characters, four regular enemy species, three boss identities, and three routes
- Real 3D meshes, skeletal animation, floor-ray aiming, lighting, and shadows
- Seven ball materials, five evolutions, relic choices, and precision-return attacks
- Four-direction movement in the quarry, plus two classic horizontal-movement routes
- Finite elite armor, interruptible boss cores, staged enemy entrances, and danger warnings
- Practice, an upgrade journal, run history, pause, suspend/resume, and independent music/SFX settings
- Synthesized battle music and event-driven combat audio

The in-game interface is currently primarily Simplified Chinese. English-first documentation does not mean the game has an English localization.

## Getting started & controls

Download the Windows package from the project page, extract it, and run the included game executable. This documentation-only repository cannot be cloned and run as the game.

- **Mouse:** aim; auto-fire is enabled by default
- **WASD / arrow keys:** move in the quarry; classic routes use horizontal movement
- **Tab:** toggle auto-fire; hold the left mouse button for manual fire
- **P / Esc / Space:** pause or resume during combat
- **1 / 2 / 3:** directly select an offered upgrade or relic
- **Card selection:** hover to preview, click to select, then use Confirm
- **M:** master mute · **F:** reduced effects · **F12:** screenshot
- Use the pause menu to suspend a run, then Continue from the title screen

Catch returning main balls by moving into their landing path. New quarry runs enable the current precision-return, armor, and encounter rules; restored runs retain their recorded compatibility rules. The 3D save namespace is separate from the historical 2D edition.

## Verification & limitations

The game is developed with **Godot 4.6.3**, using GDScript and the GL Compatibility renderer. Automated simulation, save, UI, audio, and packed-resource checks accompany development. Native Windows execution has not yet been verified; Windows exports have been inspected using Linux Godot.

v0.36 verification covers 11,236 focused contact-geometry assertion executions, 768 unchanged hit/catch/disabled cases, 1,800 deterministic gameplay/save/RNG frames, and 180 native comparison states. All 60 corresponding Off images are pixel-identical. Baseline/package checks matched 78 scripts, 26 runtime image/audio/font resources, and 44 model scenes. These are the v0.36 checks, not a rerun of every historical test.

The final embedded package ran in Linux Godot 4.6.3 with OpenGL Compatibility and llvmpipe. Native Windows execution remains untested. The six-second muted before/after clip contains three separately restored two-second Normal/Low/Off excerpts at a fixed 60 Hz simulation and 30 Hz capture; it does not measure real-time FPS or show an uninterrupted human playthrough. The warning-overlap image is a deliberate visual test fixture, not natural boss gameplay. Audio is unchanged and no subjective listening assessment is claimed.

## Changelog

Dates are the first successful public game-site publication times in **UTC**, where verified. They are not Git commit dates. Historical entries without a verified public timestamp are explicitly marked. The history describes earlier game builds, including the separate 2D edition; it does not mean their source or assets are included in this repository.

### v0.36 · A Clearer Wall-Contact Accent

2026-10-02 · 19:07:02.024 UTC

- Made a small readability adjustment to wall ricochets: contact strokes retain their existing position and timing, with a short pale core, stronger taper, and brief peak before fading.
- Normal effects are slightly clearer, Low stays subdued, and Off still hides the effect. Hit and catch contacts are unchanged.
- Preserved ball heads, wakes, damage, collision rules, skill effects, RNG, and save compatibility. Menu and window labels now read v0.36; the simulation/save version is unchanged.
- Verified 11,236 focused contact-geometry assertions and 768 unchanged hit/catch/disabled cases, 1,800 deterministic gameplay/save/RNG frames, and 180 native comparison states. All 60 corresponding Off images are pixel-identical. A deliberately constructed warning-overlap fixture preserved warning geometry in all three modes.
- The final embedded package was checked and exercised in Linux Godot, including resuming a v0.35 suspended run, pause/resume, upgrades, and results. Native Windows execution remains untested. The muted six-second before/after clip uses three separately restored two-second fixed-step excerpts; it is not a real-time performance test or continuous human playthrough.

### v0.35 · Clearer Skills and Projectiles

2026-10-02 · 11:07:58.428 UTC

- Replaced eleven skill icons and five fusion icons with distinct effect-shaped artwork. Compact markers retain exact ranks while removing persistent inventory frames and wide rank strips.
- Distinguished facts, benefits, costs, and previous values in upgrade and current-build descriptions. Benefit/cost labels preserve meaning without relying on color alone.
- Shorter reload intervals display as a benefit, lower stone-wear floors as a cost, and capped repairs no longer imply an extra improvement. Signs, values, conditions, and limits are preserved.
- Added compact faceted ball heads, short tapered wakes, and directional contact fragments. Wakes follow genuine ricochet waypoints rather than cutting across recorded corners.
- Low effects shorten and soften wakes. Off retains solid heads and shadows while removing wakes/contact geometry; the impact-feedback switch also suppresses contact fragments.
- Retained v0.34's minimal interface and quieter floor. Gameplay, damage, skill/fusion effects, RNG, save schema, controls, original audio, and 3D suspended-run compatibility are unchanged.
- Historical verification recorded 11,676 headless, 2,021 native Linux, 238 embedded-resource, and 1,639 packed-UI assertion executions, including repeated modes, plus six pointer checks. The muted six-second clip uses separately restored fixed-step excerpts; native Windows was untested.

### v0.34 · Minimal UI

2026-10-02 · 10:17:46.778 UTC

- Rebuilt upgrade and relic screens as three parallel, lightly framed choices with complete effects and penalties. Hover previews, the locked selection, and final confirmation remain distinct.
- Made pause and settings compact two-column layouts, keeping resume, suspend, and end-run actions visible without scrolling to the bottom. Short keycaps match the actual controls.
- Reduced heavy HUD outlines, decorative portrait space, and competing boss/combo ornament while retaining exact health, ranks, and actionable warnings. Full-screen menus fade the combat HUD and use soft local shading over the recognizable arena.
- Unified title, character/configuration, journal, help, results, suspend/replacement, and practice screens. Journal Back stays visible; current effects are distinct from next-rank previews. Results prioritize the full score and major damage sources.
- Made suspend failures visible while retaining the current run, focused Cancel by default for replacement confirmation, and aligned practice guidance with click-then-confirm or direct number-key selection.
- Retained short interruptible transitions and reduced/off-effects paths. Quarry floor emission is half its previous strength. Original models, music, sound, combat math, RNG, save format, and warning geometry/timing remain unchanged; old 3D suspended runs stay compatible.
- Separately redesigned the project page in charcoal, ivory, and coral: compact navigation and download area, update/video sections, expandable history, screenshot gallery, guestbook, getting-started steps, and footer. Historical text, first-publication times, and existing comments were preserved.

### v0.33 · Crimson Echoes

2026-10-02 · 07:49:10.350 UTC

- Rebuilt the HUD in a black, red, and warm-white comic style, with a brush-stroke title mark, bold durability numbers and red health bar, a boss badge, and a purple-and-white COMBO display on the right.
- Added glowing chamfered icons for skills and evolutions. Normal skills show their actual three-level cap; Repair shows its actual acquisition count without implying a nonexistent fourth level.
- Added matching comic bust portraits for both original robots. Skill, catch, and upgrade messages take priority; decorative portraits hide when space is limited.
- Retained hover/press feedback, interruptible panel transitions, the settling health trail, and short combo pulses. Redrew the pause button and expanded the HUD's aim-exclusion area so hovering over the interface preserves the current aim direction.
- Replaced the player's ground marker with stable warm-white corner marks that stay distinct from frost trails. Existing characters, camera, collision, combat values, warning shapes/timing, RNG, saves, and audio remain unchanged.
- Checked 1180- and 960-wide layouts, dense inventories, large numbers, reduced/zero effects, and pause/upgrade interaction. The final validation recorded 8,465 passing assertion executions, including repeated modes and 212 packed-resource checks. Native Windows OS execution remains untested.

### v0.32 · Interaction Echoes

2026-10-02 · 06:41:16.216 UTC

- Replaced all nine character and boss models with independently redesigned 3D originals, including Cairn Courier and Flux Weaver. Added a stable thin player outline and ground marker while preserving collision geometry, attack cadence, and save identifiers.
- Added interruptible pause/journal fades, button hover/focus/press feedback, immediate HP numbers with a smoothly settling health trail, and brief combo/skill-acquisition motion. Reduced and zero-effects modes retain essential information.
- Grouped audio, music, and display settings in the pause screen, moved detailed combat rules to the journal, and separated upgrade-card type icons, levels, and actual value changes.
- Gave normal, fire, frost, and arc balls distinct silhouettes and compact trails. Real direct hits trigger a brief local flash; damage-over-time does not repeatedly flash. Existing danger warnings remain readable.
- Added quiet select/back/confirm sounds within the existing five-voice pool. The original four music stems smoothly change arrangement in response to real warnings and living bosses, preserving the continuous beat.
- Removed old downloaded images and previous character models from the runtime package; font and music notices are included with the game. Combat math, RNG, and old 3D-save compatibility remain unchanged.
- The final build passed 7,144 automated assertions/resource checks in total. Native Windows OS execution remains untested; source code and assets are still not uploaded to this README-only repository.

### v0.31 · Slate Quarry

2026-10-02 · 04:59:17 UTC

- Reworked the quarry into cool slate floors and deep-blue rock walls, reducing seam contrast while preserving arena geometry, camera, models, and collision positions.
- Organized combat information into a left-side HUD, with coral durability and amber experience bars, three skill columns for up to six skills and four columns for larger builds.
- Unified button hover, pressed, and focus colors; checked the 960×600 layout. Further transition animation remains future work.
- Includes the previously unreleased v0.30 player-hurt audio fix: actual positive HP loss can use an idle voice in the existing five-voice pool. Stale, paused, muted, or unfocused cues are not replayed. A fully occupied pool may still omit a cue.
- Combat values, enemies, build rules, RNG, and save format were preserved.

### v0.30 · Unreleased intermediate revision

The actual-player-hurt audio repair was incorporated into v0.31. v0.30 was not published as a separate release; it has no standalone public-release date.

### v0.29 · Action Feedback

2026-10-02 · 03:41:29 UTC

- Restored real HP-loss, successful interrupt, formation-break, exit-damage, and catch-multiplier feedback in the 3D renderer.
- Prioritized important action text within a combined 12-label limit; ordinary damage numbers make room for critical messages.
- Kept information visible with low or zero effects and mute, and positioned compact-window text around the HUD and boss warning area.
- Preserved combat math, cadence, drops, RNG, and 3D format-4 saves.

### v0.28 · Build at a Glance

2026-10-02 · 02:52:47 UTC

- Replaced the long skill text list with four-column skill icons, actual levels, and evolution symbols.
- Added hover details while retaining the previous aim direction over the UI; the journal remains available.
- Added brief floor markers to actual surviving members of the second-layer two-turtle/two-goblin entry. Markers fade within six seconds and remain below danger warnings.
- Preserved combat, spawning, drops, and 3D format-4 saves.

### v0.27 · Staged Entrances

2026-10-02 · 01:46:26 UTC

- New quarry runs start with six seconds of charging goblins before mixing in skeletons.
- The second layer introduces two turtles and two goblins through real free entry positions; previous-wave survivors remain.
- The last three seconds of the first two layers pause new reinforcements and remove the low-population descent speed-up. Existing threats remain active.
- Saves retain each run’s encounter rules. Later layers, classic routes, and per-species HP, damage, attack intervals, and XP rewards remain unchanged.

### v0.26 · Ordered Fractures

2026-10-02 · 01:07:47 UTC

- The quarry boss changes from a single longitudinal fracture to longitudinal-then-crosswise at 65% HP, and reverses the new sequence at 30% HP. Active attacks keep their original order.
- Breaking the 64-HP side core before the first strike cancels the group and grants the existing four-second double-damage window; direct dodging remains possible.
- Added numbered floor warnings, separate countdowns, real hammer/channel animation, and a safety-path check that can delay admission.
- The boss stops during wind-up; new ordinary attacks and reinforcements pause during grouped warnings, while existing enemies and projectiles remain.
- Old 3D saves retain their previous boss rules. No blanket enemy-stat inflation or forced invulnerability was added.

### v0.25 · Elite Armor and Ball Motion

2026-10-02 · 00:09:08 UTC

- Gave a small existing subset of elites finite armor: 30% of maximum HP, capped at 40, absorbing at most half of direct damage. Main balls wear armor three times as fast; poison/burn damage bypasses it.
- Added skeletal armor plates, an armor bar, local cracks, and feedback on actual breakage.
- Added low visual ball arcs, ground shadows, bounded trails, and contact rings while retaining ground-plane collision truth.
- Old saves keep the unarmored rules; pause, upgrade, and resume do not refill armor. Reduced effects preserve threats and armor state.

### v0.24 · The 3D Expedition

2026-10-01 · 22:59:02 UTC

- Migrated two playable characters, four normal enemy species, three boss identities, and all three routes to real modeled 3D scenes, with 44 model-catalog entries.
- Added floor-ray aiming, lighting, shadows, layered locomotion/throw animation, enemy hit/channel/freeze/death presentation, and honest collision warnings.
- Migrated practice, upgrades, relic confirmation, the journal, history, settings, pause, suspend, and resume.
- Preserved existing combat systems and music. The 3D save namespace is independent from the separately retained v0.23 2D game.

### v0.23 · Precision Return · 2D Archive

2026-10-01 · 21:16:04 UTC

- New quarry runs can charge one main ball by moving at least 72 px from the previous successful charge position and catching within ±24 px of the catch center.
- The first actual hit within three seconds deals 1.5× damage, with a global four-second cooldown. The charge does not stack, transfer, or refresh.
- Added a readiness ring, timer, and feedback only for an actual precision hit. Damage-over-time, split balls, arcs, and evolution bonus damage do not inherit the multiplier.
- Pause and suspend preserve ownership and timers; old saves keep their previous rules.

### v0.22 · Damage Icons, Status Outlines, and Boss Health

2026-10-01 · 20:21:08 UTC

- Added distinct icon silhouettes and colors for 12 actual damage sources, with smaller damage-over-time labels and a 12-label cap.
- Tied local burn, poison, slow, and freeze outlines to real status durations; low effects retain status markers without animated rim light.
- Added the boss name, live HP, phase ticks, and a delayed health trail near the upper center.
- Combat and RNG remained unchanged; this version did not add precision criticals or elite-armor mechanics.

### v0.21 · Movement and Active Threats

2026-10-01 · 19:39:07 UTC

- New quarry runs support WASD/arrow-key four-direction movement with normalized diagonals and relative-motion catches.
- Added warned goblin charges, skeleton fans, turtle bolts, and delayed shaman blasts, with bounded concurrent threats.
- Locked blasts stop tracking; attacks or freeze can interrupt channels. Contact damage uses brief protection windows.
- Moved the exit defense line to the lower boundary. Old suspended runs retain horizontal movement.

### v0.20 · Quarry Materials

2026-10-01 · 18:20:09 UTC

- Reorganized the 2D rock backdrop into larger value groups and quieter textures, with cached background treatment.
- Added restrained grounding and front-edge shading to enemy platforms.
- Preserved positions, collision, character scale, movement, attack rules, values, and RNG.

### v0.19 · Card Confirmation and Boss Reference

2026-10-01 · 17:24:37 UTC

- Hovering previews a card; clicking or directional selection commits a choice, and the confirmation button names the selected upgrade or relic.
- Crossing another card while moving to Confirm no longer replaces the selected item. Rerolls reset selection; returning from the journal preserves it.
- Added pause-screen reference information for the current boss core/counterattack rules, reducing duplicate combat instructions.

### v0.18 · Five Evolution Signatures

2026-10-01 · 16:47:01 UTC

- Added distinct bounded impact outlines for Miasma, Comet, Cinder, Stormglass, and Forked effects.
- Feedback responds only to real positive non-periodic evolution hits, coalesces dense events, and respects reduced/zero effects.
- Danger warnings, hostile projectiles, and core information stay visually above friendly effects. Combat and RNG are unchanged.

### v0.17 · Counterattack Choices

2026-10-01 · 15:13:49 UTC

- New quarry runs can break a 64-HP side core during a 2.4-second wind-up to cancel its red lane and expose the boss to double damage for four seconds.
- The core grants no extra XP, kills, or score; direct dodging remains an option.
- Upgrade descriptions explain the choice’s direction, conditions, alternatives, and remaining evolution ingredients. Old saves retain their rules.

### v0.16 · First-Acquisition State

2026-10-01 · 13:37:43 UTC

- First acquisition of Stone resets only its existing main-ball wear; first acquisition of Comet makes surviving main balls ready while retaining Stone wear.
- Further levels, pause, and resume do not repeat the first-acquisition initialization.
- Saves record each run’s rules and show compatibility information.

### v0.15 · Visible Upgrade Feedback

2026-10-01 · 12:51:50 UTC

- Added exact skill/level and evolution-recipe feedback on acquisition or reinforcement.
- Added concise visual and synthesized audio responses to a skill’s first real effect, plus persistent evolution indicators and hover details.
- Pending feedback survives modal pauses; loading old saves does not replay past rewards. Empty targets and ineffective events do not count as successful first effects.

### v0.14 · Impact Rhythm and Layered Music

2026-10-01 · 12:37:24 UTC

- Added original four-layer battle music that responds to actual kills, catches, and armor breaks.
- Added bounded, coalesced impact, kill, combo, catch, pickup, and shot audio, plus XP-bar pulses and optional restrained camera emphasis.
- Preserved running animation during continuous attacks and added independent music/SFX volume and master mute.

### v0.13 · Ordered Collision and Render Optimization

Historical record; public date unverified

- Cached static quarry walls, batched a fixed-capacity ball display, and reduced decorative drawing.
- Preserved threat warnings, character animation, ball cores, and combat values.
- Fixed the optional training scene using the wrong quarry background.

### v0.12 · Characters and the Descending Quarry

Historical record; public date unverified

- Introduced the projected quarry route and dense descending enemy formations while retaining both earlier routes.
- Added two playable character identities with distinct starting styles, portrait presentation, and supplied animation assets in the historical 2D edition.
- Reorganized the combat HUD, aggregated damage numbers, and clarified threat markers.

### v0.10 · Moonlit Dungeon and Safe Suspension

Historical record; public date unverified

- Reworked the historical 2D dungeon, character/skill UI, and combat information layout.
- Added pause-to-suspend and continue while protecting prior save data.

### v0.8 · Relic Trade-offs

Historical record; public date unverified

- Added six relics with benefits and costs, with at most two chosen per run.
- Added one optional skill reroll, combination previews, and relic records.

### v0.7 · Ritual Chamber

Historical record; public date unverified

- Added a second route, a three-prism layout, and mirrored formations.
- Added casters, warned charging enemies, and a shaman boss with destructible nodes.

### v0.6 · Performance and Stability

Historical record; public date unverified

- Cached the static corridor and batched trails and particles.
- Added a reversible reduced-effects mode that preserves ball cores and danger warnings.

### v0.5 · Corridor Depth and Interactive Practice

Historical record; public date unverified

- Reworked corridor lighting and combat feedback, and added four-stage interactive practice.
- Added volume, effects, shake, and brief visual hit-stop settings.

## 简体中文

REBOUND《深渊回响》是一款使用 Godot 制作的实时弹射肉鸽原型。向推进的敌阵发射弹珠，走位接回回落的主弹，组合升级，并在三条 3D 路线中应对不同威胁。

[项目页与 Windows 下载](https://rebound-game.dio-world.chatgpt.site) · [English](#repository-status) · [中文更新日志](#中文更新日志)

### 仓库状态

**本仓库目前只有这份 README，暂不上传代码、模型、其他素材和构建文件。**

- **最新公开游戏版本：v0.36 · 墙面反弹的小幅清晰度优化**，首次公开于 2026-10-02 19:07:02.024 UTC（北京时间 10 月 3 日 03:07）
- 小幅强化墙面反弹瞬间，保留 v0.35 的 16 个技能/进化图标、语义数值标识和紧凑弹珠效果
- 项目页同步换为炭黑、米白与珊瑚色设计，覆盖下载、更新、截图和留言区域
- 游戏下载、实机片段和截图见上方项目页
- 本项目是桌面游戏，不是网页即玩游戏

### 游戏内容

- 两名可玩角色、四类常规敌人、三位 Boss 与三条路线
- 真实 3D 网格、骨骼动画、地面投射瞄准、灯光和阴影
- 七种弹珠材料、五种进化、圣物选择与精准回击
- 矿渊四向移动，以及两条经典横向移动路线
- 有限强化护甲、可打断的 Boss 地核、分段入场和危险预警
- 练习、图鉴、战绩、暂停、暂存继续，以及独立音乐/音效设置
- 合成战斗音乐与真实事件驱动音效

游戏内界面目前主要为简体中文，英文优先文档不代表已完成英文界面本地化。

### 开始游戏与操作

在项目页下载 Windows 包，解压后运行其中的游戏程序。本仓库只有文档，克隆后不能直接运行游戏。

- **鼠标**：瞄准，默认自动射击
- **WASD / 方向键**：矿渊四向移动，经典路线横向移动
- **Tab**：切换自动射击；关闭后按住鼠标左键手动射击
- **P / Esc / 空格**：战斗中暂停或继续
- **1 / 2 / 3**：直接选择升级或圣物
- **选牌**：悬停预览，点击选定，再按确认
- **M** 总静音 · **F** 低特效 · **F12** 截图
- 暂停菜单可暂存本局，标题页可继续

走到回落主弹的落点接回弹珠。新矿渊远征使用当前精准回击、护甲和遭遇规则；恢复旧暂存时保留该局记录的兼容规则。3D 存档与历史 2D 版独立。

### 验证与限制

开发引擎为 **Godot 4.6.3**，使用 GDScript 与 GL Compatibility 渲染器。开发过程中进行模拟、存档、界面、音频和打包资源检查。Windows 包已通过 Linux Godot 下的导出资源检查，但尚未完成原生 Windows 系统运行验证。

v0.36 验证包括 11,236 次接触几何断言执行、768 个保持不变的命中/接回/关闭特效用例、1,800 帧玩法/存档/随机数一致的固定输入回放，以及 180 帧状态一致的原生对比；其中关闭特效的 60 帧图像逐像素一致。基线/打包检查匹配 78 个脚本、26 个运行时图片/音频/字体资源和 44 个模型场景。这些是本轮 v0.36 的验证范围，不代表重新运行了全部历史测试。

最终内嵌包在 Linux Godot 4.6.3、OpenGL Compatibility 和 llvmpipe 下运行，尚未进行原生 Windows 实机测试。6 秒无声前后对比片由标准/低/关闭三段分别恢复存档的 2 秒片段组成，模拟固定 60 Hz、采集 30 Hz，不代表实时帧率或连续人工游玩。危险区域重叠图是刻意构造的视觉验收场景，并非自然首领实战；音频未改动，未作主观听感评价。

## 中文更新日志

有证据时，下列时间采用游戏站首次成功公开发布的 **UTC 时间**，并非 Git 提交时间。未确认公开时间的早期版本标为历史记录，不补造日期。日志描述历史游戏版本，包括独立的 2D 版，并不代表本仓库包含其源码或素材。

### v0.36 · 墙面反弹的小幅清晰度优化

2026-10-02 · 19:07:02.024 UTC

- 小幅调整墙面反弹的可读性：接触笔触仍在原有碰撞位置和时刻出现，增加短促浅色亮芯、更明显的渐细，以及淡出前的短暂峰值。
- 标准特效更清楚一点，低特效保持克制，关闭特效仍不显示；命中和接回的接触效果保持不变。
- 弹珠本体、尾迹、伤害、碰撞规则、技能效果、随机数和存档兼容性不变。菜单与窗口标记统一为 v0.36，模拟/存档版本标记保留。
- 通过 11,236 次接触几何断言执行，768 个命中/接回/关闭特效用例保持不变；1,800 帧固定输入回放的玩法/存档/随机数一致，180 帧原生对比状态一致，关闭特效的 60 帧图像逐像素一致。刻意构造的危险区域重叠测试在三种模式下均保留原预警几何。
- 最终内嵌包已检查，并在 Linux Godot 中操作继续 v0.35 暂存、暂停/继续、升级和结算；原生 Windows 仍未测试。6 秒无声前后对比由三段分别恢复存档的 2 秒固定步进片段组成，不代表实时性能或连续人工游玩。

### v0.35 · 技能与弹珠更清晰

2026-10-02 · 11:07:58.428 UTC

- 11 个技能与 5 个进化图标改为独立的效果造型，保留精确等级的小标记，移除常驻外框与整条等级条。
- 升级与当前构筑说明区分事实数值、收益、代价和旧值，收益/代价同时带有文字标识，不仅依赖颜色。
- 更短的齐射间隔标为收益，更低的岩芯磨损下限标为代价；修复已达上限时不再暗示额外提升。符号、数值、条件和限制均保留。
- 弹珠加入紧凑立体切面、短而渐细的尾迹和方向性接触碎片，尾迹沿真实碰撞拐点绘制，避免跨过已记录的反弹转角。
- 低特效缩短、减弱尾迹；关闭特效保留实体弹珠和阴影，移除尾迹与接触碎片；命中反馈开关也控制接触碎片。
- 保留 v0.34 简洁界面与较安静的地面。玩法、伤害、技能/进化效果、随机数、存档格式、按键、原有音频及 3D 暂存兼容性未改动。
- 当时记录 11,676 次无界面、2,021 次原生 Linux、238 次内嵌资源及 1,639 次打包界面断言执行，包含重复模式，另有六项鼠标检查。6 秒无声短片由分别恢复的固定步进片段组成，原生 Windows 当时未测试。

### v0.34 · 简洁界面

2026-10-02 · 10:17:46.778 UTC

- 升级与遗物改为并排三选项，弱化边框，完整展示真实效果与代价；悬停预览、已选项和最终确认分开。
- 暂停与设置采用紧凑双栏，继续、暂存和结束本局等主要操作无需滚到页面底部；短键帽与真实操作一致。
- 战斗 HUD 减少厚重描边、装饰画像和过强的首领/连击装饰，保留准确耐久、等级与关键提示。全屏菜单淡出战斗 HUD，以柔和局部遮罩保留可辨认的场景。
- 标题、角色与配置、图鉴、帮助、结算、暂存/替换确认和练习统一简洁层级。图鉴返回按钮固定可见，当前效果与下一等级预览分开，结算突出完整得分和主要伤害来源。
- 暂存失败明确提示并保留当前战局，替换暂存默认聚焦取消；练习说明准确对应点选后确认或直接按数字键的行为。
- 保留短促可中断动效，以及低特效/关闭特效路径。矿渊地板自发光减为此前一半。原创模型、音乐、音效、战斗数值、随机数、存档格式和危险预警几何/时序保持不变，旧 3D 暂存继续兼容。
- 项目页另行完成炭黑、米白与珊瑚色改版，覆盖导航、紧凑下载区、更新与视频、可展开历史、截图库、留言板、开始步骤及页尾；保留历史正文、首次发布时间和已有留言。

### v0.33 · 红影回响

2026-10-02 · 07:49:10.350 UTC

- HUD 重做为黑、红、米白配色的漫画风，加入笔刷标志、醒目的耐久数字与红色血条、首领徽章，以及右侧紫白色 COMBO。
- 技能与进化改用发光切角图标；普通技能准确显示三级上限，修复显示实际获得次数，不暗示不存在的第四级。
- 两位原创机器人增加对应的漫画半身像。技能、接回和升级提示优先显示，空间不足时隐藏装饰画像。
- 保留悬停、按下反馈、可中断界面过渡、血条余量和连击短脉冲；重绘暂停按钮，扩大 HUD 的瞄准隔离范围，悬停界面时保持当前瞄准方向。
- 玩家脚下改为稳定的米白定位角标，与冰霜轨迹区分。原有角色、镜头、碰撞、战斗数值、预警形状与时序、随机数、存档和声音保持不变。
- 检查 1180 和 960 宽度、高密度技能、大数字、低/关闭特效以及暂停和升级操作。最终验收合计 8,465 次通过的断言执行，包含重复模式和 212 项打包资源检查；原生 Windows 系统运行仍未测试。

### v0.32 · 交互回响

2026-10-02 · 06:41:16.216 UTC

- 换成九个重新独立设计的原创 3D 角色和首领，包括岩标信使、流光织者；玩家增加稳定薄描边与脚下标记。保留碰撞位置、攻击节奏和存档标识。
- 暂停和图鉴加入可中断的淡入淡出，按钮有悬停、聚焦和按下反馈；耐久数字立即更新，血条余量平滑收拢，连击和技能获得有短促动效。轻量和零特效模式保留基本信息。
- 暂停页集中音效、音乐和画面设置，详细战斗规则移到图鉴说明；升级卡片分开显示类型图标、等级和实际数值变化。
- 普通、火焰、冰霜、电弧弹使用不同轮廓与收束轨迹；真实直伤触发目标局部短闪，持续伤害不重复闪烁，保留危险预警。
- 选择、返回和确认增加安静的操作声，共用原有五个声部；原有四条原创音乐声部根据真实预警与存活首领平滑调整层次，保持连续节拍。
- 运行包移除旧下载图片与旧角色模型，随包提供字体和音乐许可说明；战斗数值、随机数和旧 3D 暂存兼容性保持不变。
- 最终版本合计通过 7,144 项自动断言与打包资源检查。尚未在原生 Windows 系统运行；本 GitHub 仓库仍只有 README，未上传代码或素材。

### v0.31 · 冷岩矿渊

2026-10-02 · 04:59:17 UTC

- 矿道改为冷灰石板与深蓝岩壁，降低地砖接缝对比，让弹珠、敌人与危险区域更突出。保留场地、摄像机、模型与碰撞位置。
- 战斗界面整理为左侧信息栏：耐久与经验分别使用珊瑚红、琥珀色进度条；6项以内技能使用3列卡片，多技能自动使用4列；进化、连击和操作提示分区。
- 统一暂停按钮与菜单的悬停、按下、聚焦配色；验证960×600窗口与完整技能栏。后续继续完善过渡动效。
- 包含此前未发布的真实失血声音修复：短促下降提示音优先使用原有5个共享声部的空闲位置；过期、暂停、静音和失焦不会补播旧受伤提示。
- 战斗数值、敌人、构筑、随机数、存档格式和原有2D回退版保持不变。

### v0.30 · 未单独发布的中间修订

真实失血音效修复已合入 v0.31。v0.30 没有单独公开发布，因此不标注独立公开发布日期。

### v0.29 · 行动回响

2026-10-02 · 03:41:29 UTC

- 玩家实际失血优先显示，真实取消施法才标记打断；破阵与出口受损提示也回到3D画面
- 接回显示最近一次提示对应的真实弹珠倍率，同时动作可汇总次数；数字与动作合计最多12条，普通伤害字为关键提示让位
- 低特效、零特效和静音仍显示这些信息，小窗口提示避开固定HUD与Boss顶部预警；沿用护甲外观和破裂图标
- 战斗数值、攻击节奏、掉落、角色规则与随机数不变，3D格式4暂存继续兼容；这次修复已有信息展示，没有新增伤害机制

### v0.28 · 构筑速览

2026-10-02 · 02:52:47 UTC

- 把3D战斗HUD的长技能文字列改成四列图标与真实等级；已获得的进化也有对应图形，装配和生效事件反馈到对应图标
- 鼠标悬停可查名称与精确等级，J继续打开图鉴；停在图标上时维持原瞄准方向，避免弹珠跟着界面移动
- 第二层两龟与两哥布林增加短暂脚下角标，只跟随实际存活成员并在6秒内淡出；危险预警仍在角标上层
- 战斗数值、敌阵规则、掉落和3D格式4存档不变；16项战斗与存档源文件和v0.27逐字节一致，旧暂存继续兼容

### v0.27 · 分段入口

2026-10-02 · 01:46:26 UTC

- 第一层开场6秒先遇到冲锋哥布林，再进入骷髅与哥布林混合敌阵；冲锋保留真实预警、锁定目标与可打断规则
- 第二层让两龟与两哥布林从上方真实空位结队入场，旧波幸存者照常保留，小队可能被旧怪遮挡
- 前两层最后3秒暂停新增援军，并取消缺员时的下压加速；已有怪物、预警和飞行敌弹继续生效，仍需闪躲
- 暂存记录本局敌阵规则，旧3D远征恢复并再次暂存后仍保留原编排；第三层以后生成算法、两条经典路线及各敌种生命、伤害、攻击间隔与经验奖励不变

### v0.26 · 双裂次序

2026-10-02 · 01:07:47 UTC

- 踏碎者先用单道纵裂；生命降至65%或以下，新一组改为纵裂先、横裂后；30%或以下的新一组反序，已开始的招式不临时换顺序
- 首道生效前击碎侧面64生命地核，可取消整组裂缝并获得原有4秒Boss受伤×2窗口；也可直接走出两道危险区域
- 地面用1、2和各自倒计时标出次序，边框颜色辅助辨识；Boss有真实挥锤与吟唱动作，地核只有真正被击碎才使用破碎外观
- 蓄力期间Boss定身，整组预警时暂停新增普通攻击和增援，已有敌人与敌弹保留；出招前检查实际移速及沿途威胁，未找到已验证逃生路径时延后
- 保持Boss生命和单次攻击伤害，没有统一提高小怪生命、数量或攻击伤害，也不增加无敌阶段或最低存活时间
- 新矿渊远征启用新编排；v0.24、v0.25旧3D暂存沿用旧Boss规则并可再次暂存，两条经典路线与独立2D版保留

### v0.25 · 强化护甲与跃动弹珠

2026-10-02 · 00:09:08 UTC

- 新矿渊远征中的原有少量强化怪获得有限护甲：耐久为最大生命的30%、最多40点，最多分担一半直接伤害；主弹按3倍削甲，毒火持续伤害穿透
- 护甲使用随骨骼动作的立体甲片，附独立甲条和局部裂纹；真正归零时移除外观并触发破甲音效与反馈
- 弹珠新增低幅立体视觉弧线、地面影子、局部光带拖尾和实际墙面、命中或接球接触圈；碰撞位置和敌弹危险轮廓保持明确
- 护甲溢出、精准回击与圣物额外伤害按实际生命损失统计，吸收的护甲值不计入生命伤害
- 旧3D暂存继续无护甲的原规则，标题会提示；新局启用护甲，升级、暂停与恢复不会回满甲值
- 局部命中反馈开关准确控制对应光效和接触圈；低特效减少装饰，仍保留危险预警与护甲状态

### v0.24 · 真正 3D 远征

2026-10-01 · 22:59:02 UTC

- 44个模型目录项覆盖两位可玩行者、四类常规敌人、三位Boss、三条路线，以及场景、机关、球体和拾取物
- 新增3D镜头、地面投射瞄准、模型身体选择与灯光阴影；主角移动腿部和上半身抛球分层，敌人有受击、吟唱、冻结与死亡表现
- 保留四向矿渊、两条经典横移路线、五种进化、圣物、精准回击、伤害类型图标、状态效果、Boss血条残影及原战斗音乐
- 练习、升级与圣物确认、图鉴、战绩、设置、暂停、暂存和继续均已迁移；3D使用独立存档，不读写v0.23的2D存档
- 修正危险区与实际碰撞边界的对应关系，棱镜恢复紫晶色，矿渊地面减少碎纹，经典路线镜头用足视窗

### v0.23 · 走位接球后的精准回击 · 2D 留档

2026-10-01 · 21:16:04 UTC

- 新开深坑远征：相对上次成功充能位置移动至少72px，再从接球中心±24px接回主弹，让该球获得一次精准回击
- 充能保留3秒，首次实际主弹命中伤害乘1.5；全局4秒冷却，不叠加、不转移、不因再次接球延长
- 充能球显示短光环与倒计时；只有实际触发的精准回击显示暴击数字、短星芒和独立音效
- 持续伤害、分裂子弹、电弧和进化附伤不继承暴击倍率；结算按实际扣血计算额外伤害
- 暂停、暂存与继续保留球归属及计时；旧暂存继续原规则，新局才启用精准回击

### v0.22 · 伤害图标、状态轮廓与 Boss 血条

2026-10-01 · 20:21:08 UTC

- 12种实际伤害来源使用轮廓图标和颜色，移除岩、毒、燃、电等文字前缀；持续伤害数字较小，同屏最多12条
- 燃烧、中毒、冰缓、冻结绑定真实剩余时间，增加贴怪轮廓的局部 shader 边光；结束、死亡与换局及时清理
- 状态图标固定槽位，毒层用点数表示；低特效模式关闭动态边光但保留状态标记
- Boss在场时显示中上方姓名、真实血量和阶段刻度；扣血后金色残血短暂保留再平滑追赶
- 连击数按真实主弹命中小幅跳动，保留已有档位音效和音乐层；不改变战斗数值和随机序列

### v0.21 · 四向走位与主动敌阵

2026-10-01 · 19:39:07 UTC

- 新局支持 WASD / 方向键四向移动，斜向速度一致；回收弧线随玩家移动，相对运动判定接球
- 飞魔预警冲锋、亡骨三矛扇射、铁壳蓄力甲刺、萨满延迟咒印；独立攻击间隔并限制同屏危险数量
- 咒印锁定落点后不追踪，可攻击吟唱者或冻结打断；接触伤害配短暂受击保护
- Boss 攻击节奏略加快，裂地核反击保留；出口防线移至场地下缘并清楚标示
- 旧暂存沿用旧横移规则；请新开深坑远征体验本版四向移动

### v0.20 · 矿渊材质与像素层次

2026-10-01 · 18:20:09 UTC

- 重整岩壁的大块明暗面，减少细碎石点与苔藓纹理，保留矿渊主题、透视与开放地面
- 背景适度压暗并一次性缓存，让角色、弹珠和危险预警保持视觉优先
- 敌人地台增加轻微前侧明暗、接地阴影与边角变化，碰撞范围、角色尺寸和位置不变
- 标题与选牌沿用同一套背景材质；数值、随机序列、移动与攻击规则不变

### v0.19 · 选牌确认与 Boss 规则参考

2026-10-01 · 17:24:37 UTC

- 修复鼠标移向确认按钮时，途经另一张卡片会意外改变装配对象的问题
- 升级与圣物：悬停只预览，点击或左右键选定，按钮显示将装配的名称；确认按钮或 Enter 装配，1/2/3 保留直接装配
- 预览与已选定使用不同边框和文字，重复点击卡片不会直接装配；重抽和新选择清除旧选定，图鉴返回保留选定
- 当前规则的深坑 Boss 战新增暂停参考：裂地核 64 耐久、2.4 秒窗口，击碎取消对应红带并使 Boss 受伤 ×2 持续 4 秒，也可侧移闪避
- 裂地核出现时移除底部重复指令，保留顶部规则与局部耐久、倒计时；移动、战斗数值、掉落、抽牌和随机序列不变，旧局保持原规则

### v0.18 · 五种进化的局部光效

2026-10-01 · 16:47:01 UTC

- 五种进化加入不同命中轮廓：瘴雾双弧、霜陨坠击、烬火花瓣、雷晶冰芒、分形电枝
- 光效只响应真实、正值、非持续跳伤的进化命中，密集伤害合并显示并限制频率
- 轻量模式关闭柔光与填充面，最多保留三组简明轮廓；零特效不绘制新增光效
- 危险预警、敌弹和裂地核耐久与倒计时始终显示在友方特效上方
- 伤害、经验、掉落、构筑与随机序列不变，旧局保留原规则，读档不补播过去的命中光效

### v0.17 · 转火反打与选牌方向

2026-10-01 · 15:13:49 UTC

- 新开深坑远征时，裂地冲击会出现侧面的裂地核：64 耐久，2.4 秒窗口
- 击碎裂地核可消除对应红带，让首领承受 2 倍伤害、持续 4 秒；也可以继续攻击并侧移闪避
- 所有伤害来源都能命中裂地核；它不额外奖励经验、击杀或分数
- 升级选项标出接回爆发、群体传导、控制增伤等方向，说明生效条件与限制
- 详情显示其他可选方向，以及距离进化还差几级素材
- 旧暂存继续沿用旧规则；需要新开一局体验本版首领机制，暂停页会标明本局规则

### v0.16 · 首次装配不背旧账

2026-10-01 · 13:37:43 UTC

- 首次获得岩芯弹时，只重置现有存活主弹的岩芯磨损
- 首次获得霜陨重击时，让现有存活主弹进入就绪状态，同时保留已有岩芯磨损
- 后续升级、暂停与读档不会重复刷新首次装配状态
- 首次真实生效提示更及时，移除重复装配提示，保留危险预警
- 新开一局使用本版规则；旧暂存继续使用原规则，暂停页明确标注
- 保存格式记录本局规则，避免旧程序误读新暂存

### v0.15 · 看得见的升级回响

2026-10-01 · 12:51:50 UTC

- 装备或强化时显示准确的技能与等级，进化后显示对应配方
- 首次产生真实技能效果时，给出简短提示、图标脉冲与原创音符回应
- 五种进化加入小型常驻标识、悬停说明与首次命中位置标记
- 暂停或连续选择时保留待显示提示，恢复旧存档不会重播旧奖励
- 空目标、无伤害爆炸和中毒刷新不会被误报为首次成功生效

### v0.14 · 打击节奏与连击音乐

2026-10-01 · 12:37:24 UTC

- 加入原创四层战斗音乐，随真实击杀、接回与破甲事件变化
- 补全命中、击杀、连击、接球和拾取音效，密集事件合并处理
- 增加经验条脉冲、有限命中刻线与可关闭的轻量镜头强调
- 修复连发动画反复重置，保留移动射击的跑步动作
- 新增独立音乐 / 音效音量与总静音，兼容旧存档

### v0.13 · 保序碰撞与矿渊渲染优化

历史记录；公开日期未确认

- 缓存静态矿壁，固定容量弹珠批次，减少装饰绘制
- 保留敌方预警、球体亮芯、角色动画与玩法数值
- 修复可选训练误用矿渊背景，保持原路线可选

### v0.12 · 行者与沉降矿渊

历史记录；公开日期未确认

- 加入默认投影矿渊与密集敌阵，原两条路线仍可选
- 两名真实动画角色、原创肖像与独立出发风格
- 重做边缘战斗 HUD、聚合伤害数字与敌方预警

### v0.10 · 月光玩具箱与安全暂存

历史记录；公开日期未确认

- 重做地牢画面、角色与技能界面，调整战斗信息布局
- 加入暂停暂存与继续游戏，保留本局状态并保护旧档

### v0.8 · 圣物取舍

历史记录；公开日期未确认

- 加入六件带收益与代价的圣物，每局最多选择两件
- 增加一次可选技能重抽、组合预览与圣物记录

### v0.7 · 秘仪祭室

历史记录；公开日期未确认

- 加入第二条路线、三棱镜布局与镜像编队
- 新增施法者、预警冲锋敌人与带可摧毁节点的萨满首领

### v0.6 · 性能、批量绘制与长期稳定性

历史记录；公开日期未确认

- 缓存静态回廊并批量绘制拖尾与粒子
- 新增可逆轻量模式，保留弹珠亮芯和危险预警

### v0.5 · 回廊纵深、训练引导与细化反馈

历史记录；公开日期未确认

- 重绘回廊光影与战斗反馈，加入四段交互引导
- 提供音量、特效、震动和短促视觉顿帧设置

