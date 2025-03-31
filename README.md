# TDS-Project-2

## Project Overview
This project is part of the Tools in Data Science course at IIT Madras' Online Degree in Data Science program. The goal is to build an LLM-based application that can automatically answer questions from the course's graded assignments.

## Features
- API endpoint that accepts questions from 5 graded assignments
- Support for file attachments in multipart/form-data format
- JSON response with direct answers for assignment submission

## API Specification

### Endpoint
```
POST https://your-app.vercel.app/api/
```

### Request Format
- Method: POST
- Content-Type: multipart/form-data
- Parameters:
  - `question`: The assignment question text
  - `file`: Optional file attachment (e.g., CSV files)

### Example Request
```bash
curl -X POST "https://your-app.vercel.app/api/" \
  -H "Content-Type: multipart/form-data" \
  -F "question=Download and unzip file abcd.zip which has a single extract.csv file inside. What is the value in the "answer" column of the CSV file?" \
  -F "file=@abcd.zip"
```

### Response Format
```json
{
  "answer": "1234567890"
}
```

## Project Requirements

### Repository Requirements
1. Public GitHub repository
2. MIT LICENSE file
3. Complete source code
4. Deployment URL

### Evaluation Criteria
- Repository must be publicly accessible
- Repository must have an MIT license
- 5 random questions from graded assignments will be tested
- Each correct answer is worth 4 marks
- Total score is the sum of marks (no normalization)

## Timeline
- Project Due: March 31, 2025 (End of Day IST)
- Results Announcement: April 15, 2025

## Questions
For any questions about the project, please refer to the course's Discourse thread.

## License
This project is licensed under the MIT License - see the LICENSE file for details.