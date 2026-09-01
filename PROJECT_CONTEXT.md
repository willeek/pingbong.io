# pingbong.io - Project Context

## Overview
Single-file HTML5 canvas game (`index.html`) - a two-player penalty shootout / pong-style game with green-on-black retro styling.

## Game Structure
- **Ball**: Bounces between two goalkeepers; scores when passing left/right edge
- **goalkeeper1** (left): x=20, controlled by player 1
- **goalkeeper2** (right): x=canvas.width-40, controlled by player 2
- Particle effects on collisions; Web Audio score sound

## Controls (updated 2026-09-01)
| Player | Side | Keyboard | Touch |
|--------|------|----------|-------|
| Player 1 | Left | **W** (up), **S** (down) | Tap upper/lower half of left side |
| Player 2 | Right | **Arrow Up**, **Arrow Down** | Tap upper/lower half of right side |
| Start game | - | **Enter** | Tap canvas |

Previously left used Arrow Left/Right; changed to W/S for two-player keyboard play without key conflicts.

## Tech
- Pure HTML/CSS/JS, no build step or npm
- Canvas: 600x400, responsive wrapper max 600x400
- Deployed on Railway (static file serve)

## Recent Changes
- 2026-09-01: Keyboard controls split - left W/S, right arrow up/down
