# Nimbus Run Support Dataset
A synthetic dataset for a multi-agent RAG project (Enterprise Support Copilot).
Nimbus Run is a FICTIONAL managed container platform. All content is synthetic and written for learning; it contains no real customer data.

## Contents
- `docs/` : 16 markdown knowledge-base documents (unstructured data for RAG).
- `tickets.csv` : 300 synthetic support tickets (structured data for the SQL agent).
  Columns: ticket_id, created_date, category, priority, status, region, customer_plan, service_name, description, resolution, resolution_hours.
- `eval/eval_questions.csv` : 45 evaluation questions (document, tickets, both, unanswerable) with expected answers and sources.

## Notes
- Document facts are deliberately specific (limits, timeouts, roles) so retrieval is easy to verify.
- Ticket answers in the eval set were computed from tickets.csv at generation time. If you edit the CSV, regenerate or recheck them.
- Resolution fields are blank for Open and In Progress tickets.
- Disclose in your README that the data is synthetic.
