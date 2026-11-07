1. Dispatcher
- Download data from the RPA Challenge portal.
- Save the downloaded data locally.
- Add each record to the Orchestrator Queue.
- Assign a unique reference to each transaction.
2. Performer
- Open the RPA Challenge portal.
- Click the Start button.
- Retrieve transactions from the Orchestrator Queue.
- Process each transaction in the portal.
3. Failure handling
- If any transaction fails, consider the entire execution unsuccessful.
- Mark all items in the batch as System Exception (SE).
- Apply the same failure reason to all affected items.
- Re-dispatch the complete dataset to execute the challenge again.
4. Successful execution
- Confirm that all transactions are successful.
- Capture a screenshot of the final result as execution evidence.
