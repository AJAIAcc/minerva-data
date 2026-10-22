# minerva-data

Minerva's Greek and Latin data, fetched by her server (`server/classics_fetch.py` in AJAIAcc/minerva):

- `classics.db` — the Perseus canonical Greek and Latin texts and First1KGreek by citation, indexed by lemma, form and
  feature (with the Perseus English translations); Smyth's Greek Grammar and Allen & Greenough by section; the Perseus
  AGLDT and PROIEL treebanks; hypotactic.com scansions. Built by `classics/build_*.py`.
- `tagger_grc.npy`, `tagger_lat.npy` — the context tagger (`classics/train_tagger.py`).
- `data/*.db` — Hermeneus's databases (Morpheus analyses, paradigms, LSJ, Lewis & Short).

Files are split into parts under 95 MB; `manifest.json` lists them with SHA-256 checksums.
Sources keep their licences: Perseus texts, lexica, A&G and AGLDT CC BY-SA; PROIEL CC BY-NC-SA (personal use);
hypotactic Greek CC BY, Latin CC BY-SA.
