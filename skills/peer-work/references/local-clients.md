# Client notes

Use a model and client that can experience the work: a peer reviewing a motion design needs to see it move; one testing a proposed theorem needs the assumptions and the counterexample. Check which models are actually available in that client when price, quota or capability could change the choice.

For an independent reading, pass the user's original request directly to a fresh CLI session with access to the source material within the user's authorized scope. Resume that session to exchange views. A CLI may label your follow-up `user`, so identify your own comments as coming from a peer.

For Gemini in a workspace where the user runs unattended sessions with full tool access, launch `agy --model "$model" --dangerously-skip-permissions -p "$request"` from the project directory. Use the user's chosen profile when the task has narrower permissions. Bare `agy -p` cannot prompt for a tool in headless mode and can report `SUCCESS` with an empty reply after a denial.

In Codex, Composer Prediction can suggest a next step within the user's request. Treat the suggested words as the client's guess until the user sends them.

Resume the conversation when the client supports it. If a provider change prevents resuming, or recent turns are missing, start on the requested route with the original request, the work as it stands, and the version any feedback referred to. If a client says the call succeeded, check that the reply or requested edit is actually there.
