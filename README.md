# Adobe Round 1A Submission

## Submitted File

- `adobe_challenge1a.zip` contains:
  - `Dockerfile`
  - `process_pdfs.py`
  - `requirements.txt`
  - `README.md` (inside the ZIP too)
  - `sample_dataset/` with test PDFs and output

## How to Run

To build and run the Docker image:

```bash
docker build -t round1a .
docker run --rm -v "$(pwd)/sample_dataset:/app/sample_dataset" round1a
