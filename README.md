# Action Gap Bridge — participant survey

Static survey page for a study on how people judge simulated robot navigation in a
hospital environment. Final-year project, King's College London.

**Live:** https://saninja2134.github.io/ActionGapBridgeSurvey/

## Contents

| file | purpose |
|---|---|
| `index.html` | the whole survey — trajectory players, stimulus images and questions are inlined |
| `config.js` | optional override for the submission endpoint |

`index.html` is self-contained: the floor plan, the recorded trajectories and the
camera stills are all embedded, so the page has no external dependencies and works
offline. The submission endpoint is baked in at build time; `config.js` can override
it without rebuilding.

## Responses

Answers are collected client-side and POSTed as a single anonymous JSON payload. If
the endpoint is unreachable the page tells the participant their answers were not
saved and offers a download — it never reports success it cannot verify.

No response data is stored in this repository.

## Ethics

Participation is anonymous and voluntary; no identifying information is requested.
Approved under KCL REMAS, ref MRSU-25/26-58376. Contact details are on the
information sheet at the start of the survey.
