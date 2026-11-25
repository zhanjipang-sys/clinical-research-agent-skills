# Surgical 3D keyframe dispatch

## Executor rule for complex flap spatial movement (user-set 2026-11-05)

- Any scene whose core difficulty is complex spatial movement of a flap — transposition, rotation about a pivot or pedicle, book-page elevation on an uncut base, tunnel passage, subcutaneous pedicle deformation, interdigitation of two flaps — must be authored personally by Claude Code Opus (the current best Opus, 5.5 lineage or its successor), never by a generic sub-agent worker and never by another model.

- Evidence: on 2026-11-03 the v1 and v2 keyframe sets for bilobed, nasolabial, island and Z-plasty flaps, authored by non-Opus executors, were rejected wholesale by the user as surgically wrong despite geometric self-consistency; the Opus-authored batch3 sets (island pilot first, then bilobed, nasolabial, Z-plasty, each reference-first) passed the user's review on 2026-11-04/05 as accurate.

- Generic workers may only do mechanical work around these scenes (file checks, frame counts, compare-sheet compositing, uploads). Scene code, geometry and transfer mechanics are Opus-only, no exceptions and no substitutions when the Opus window is exhausted — stop and report instead.

- Run these Opus scenes serially, one scene owning the session window at a time; two parallel Opus scene builds burn the 5-hour window and freeze each other.

## Relaxation for schematic / mechanics keyframes (user-set 2026-11-05, after three Antigravity comparison tests)

- Keyframes whose core difficulty is schematic geometry or spec-driven mechanics — flat-plane designs such as Z-plasty limb geometry, or suture needle-path diagrams on layered tissue blocks such as the five-layer tension-reduction suture paths — may be authored by Gemini 4 Argon in Antigravity instead of Opus, under the same clean-room discipline: design spec and traceable references only, no Opus code or outputs, deliverables are the keyframe set plus a spec-referenced self-check and an honest receipt, and the assistant verifies every frame personally before reporting.

- Scenes that depend on organic anatomical form (nose, ear, eyelid contours) or on complex spatial movement of a flap stay Opus-only under the rule above. Gemini's bilobed test got the design and mechanics right but rendered the nose abstractly; its Z-plasty and tension-suture sets matched the Opus standard on spec compliance.

- Evidence: three same-input comparison tests on 2026-11-05 graded bilobed = approaching, Z-plasty = at standard, tension-suture = at standard; the user relaxed the rule the same day. This relaxation covers keyframes; full-render production assignments still follow the user's standing video executor rule unless the user says otherwise.

## Collect reference illustrations first

- Collect several traceable illustrations of the exact surgical procedure before any design work begins.

- Choose illustrations that show the anatomy around the operative site and the flap design in place, not generic geometry diagrams.

- Record the source of each illustration beside it so every later design choice can be traced back to a source.

- Report the gap and stop when no traceable illustration of the exact procedure can be found.

## Write a traced design specification

- Write the design specification before rendering, with each dimension and angle pointing to one collected illustration.

- Build the operative anatomy into the scene first, so a flap for a facial site reads as that anatomy and not as a flat shape.

- Model a pedicled flap as a three dimensional tissue column or tissue bridge that stays connected throughout the transfer.

- Show the design in its resting position and in its transferred position from the same camera, and compare the two views side by side.

## Review operation mechanics before rendering

- Review which sides are cut and which side stays attached before any keyframe is accepted.

- Name the carrier that moves the flap during transfer and check that it stays attached through every keyframe.

- Reject a design whose angles and positions are mathematically consistent but whose anatomy or operation mechanics do not match the references.

- Send keyframes for approval before full rendering, and hold the full render until the keyframes pass.

## Dispatch only the named executor

- Dispatch the work only to the executor the user named for this kind of build.

- Check that the named executor is available before starting, and stop with a report when it is not available or its working window is exhausted.

- Do not hand the work to a substitute worker without explicit approval, even when the substitute can start at once.

- Report the executor used and the reference comparison result in the delivery receipt, so a substitution or a skipped comparison is visible.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Alternatives for better results

- Run one pilot scene first when a new procedure type is added, and extend the method only after that scene passes its reference comparison.

- Run the teaching video acceptance checks after keyframes pass, instead of folding literature, frame count and pronunciation checks into this dispatch.

## Clinical photo base before modeling (user-set 2026-11-17)

- Every 3D flap scene must be built on a sufficient base of REAL clinical images of the actual flap transfer — intraoperative photographs, not only textbook line illustrations.

- Sources, in order of preference: open-access literature figures (PMC/StatPearls, CC-licensed), openly published clinical images on the web, and keyframes captured from surgical videos (e.g. YouTube) after watching and understanding the video — capture the frames that show design, elevation, transfer and inset.

- Register every image with its source beside it, same as illustrations. These images are modeling reference only: never republish, redistribute, or ship them inside deliverables.

- If the clinical photo base for the exact procedure is thin, report the gap and gather more before modeling; do not open modeling on geometry alone.

## Keyframe gate before any full production (user re-affirmed 2026-11-17)

- No full-length 3D video production starts before the user has reviewed and approved the keyframe set. The set must cover the WHOLE flap process: design (incision lines + pedicle), incision/elevation, transfer (including pedicle deformation/tunnel/rotation as applicable), and inset/suture — at least 1–2 frames per stage, plus a reference-vs-keyframe comparison collage.

- Preconditions in order: (1) sufficient clinical photo base registered (see section above); (2) design spec traced to references; (3) keyframes produced and sent to the user; (4) only after the user's explicit approval does full rendering begin.

- This gate applies to every flap scene, including remakes of previously approved designs when the executor or the design changes.

## Check each flap type against its own design checklist

- Write one checklist per flap type before you approve its keyframes, and check every item against the traced references.

- List every cut edge and every uncut edge for that flap type, and name the pedicle end and whether it is cut.

- Name where each dog-ear forms, and check that it falls at the original farthest end of the flap.

- For an advancement flap, cut three sides and leave the distal pedicle end uncut, with a dog-ear at each corner of the original farthest end.

- For a bilobed flap, leave the tissue bridge at the pedicle uncut.

- Design the flap slightly long to compensate for length lost in transfer, and trim the excess tip only after it is seated.

- Treat a design that exactly fills the defect as idealized geometry, and record the trim step in the design specification.

## Name flat schematics honestly

- Call a deliverable true 3D only when it shows an anatomical surface with a perspective camera, as in the batch3 standard.

- Call a flat plane design or a top view sliding animation a schematic, never true 3D.

- State in the delivery receipt whether the deliverable is true 3D or a schematic, beside the executor name.

- Do not use the true 3D label for a schematic even when its geometry checks pass.