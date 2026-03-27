# Deepface-Mirror Memory

## Current Project State
- Resolving pytest failures in `tests/unit`.
- Failures include `KeyError: 'facial_recognition'` in `test_verify.py` and `KeyError: 'face_detector'` in `test_analyze.py`.
- Additionally `FileNotFoundError` in `test_api.py`.

## Active Tasks
### Completed
1. Investigated and fixed `KeyError: 'facial_recognition'` in `test_verify.py` and `KeyError: 'face_detector'` in `test_analyze.py`. Root cause was the caching map failing to build correctly in `modeling.py`.
2. Investigated and fixed `FileNotFoundError: [WinError 3]` in `test_api.py`. Root cause was hardcoded UNIX `/tmp/` directories in integration tests.

### Next Steps
- TBD (Pending user resolution of blocked .h5 weights download to their local deepface dotfolder)

## Architectural Decisions
- TBD
