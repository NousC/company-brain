# ICP

_Who you sell to, and how every account is scored. Push it to OpenNous with `set_icp`. Weights are a judgment call: propose them, then let the operator change them._

## How the score works

score = 40 base + best-matching persona + firmographics + observed signals, clamped 0 to 100. A hard disqualifier caps the score at 25. A signal that hasn't been seen never lowers a score.

## The buyer

Two to four sentences: who the ideal customer is.

## 1. Personas (strongest single match applies)

- Best-fit role +35
- Next role +28
- Adjacent role +12
- No clear fit +0

## 2. Firmographics (these add up, when known)

- Target geography +12, secondary +4
- Target company size +12, adjacent sizes +6
- Target company type +8

## 3. Signals (observed only)

Boosts: in-market signal +12, momentum signal +8, fit signal +6

Cuts: not in market -10, wrong fit -25

## 4. Hard disqualifiers (cap the score at 25)

- Wrong market entirely
- No relevant role

## Anchors

Fit: a real example of a great-fit customer.
