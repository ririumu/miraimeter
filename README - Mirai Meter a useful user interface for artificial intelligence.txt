+--------------------------------------------------------------------+
| Mirai Meter                                                        |
| a useful user interface for artificial intelligence                |
+--------------------------------------------------------------------+

# Mirai Meter

Mirai Meter is a useful user interface for artificial intelligence.

It separates two questions that are often confused:

1. How useful can AI be for this task?
2. How much authority should AI be allowed to take?

The first question is AI contribution.
The second question is automation permission.

Mirai Meter shows both.

It does not decide the user's future.
It does not replace responsibility.
It does not turn every AI risk into a refusal.

It measures the delegation boundary.

+--------------------------------------------------------------------+
| Core idea                                                          |
+--------------------------------------------------------------------+

AI usefulness is not automation permission.

A task can be a very good use of AI while still being a poor candidate
for full automation.

Examples:

- Meeting notes:
  AI contribution: high
  Automation permission: high

- Apology message:
  AI contribution: high
  Automation permission: medium or low

- Career or life decision:
  AI contribution: high
  Automation permission: low

Mirai Meter turns this distinction into a simple UI.

+--------------------------------------------------------------------+
| What the user sees                                                 |
+--------------------------------------------------------------------+

The user enters a request.

Mirai Meter returns:

- AI contribution score
- automation permission score
- a short explanation
- what AI can safely do
- what the user or organization should confirm
- a position on a two-axis delegation map

The UI is intentionally small.

The system may be complex behind the screen, but the user-facing
question remains simple:

"How useful is AI here, and how far should it be allowed to go?"

+--------------------------------------------------------------------+
| Why this matters                                                   |
+--------------------------------------------------------------------+

Agentic AI changes the security and product boundary.

The old boundary was often:

    internet <-> firewall

The new boundary is increasingly:

    agentic AI <-> delegation

The problem is not only whether AI can answer.
The problem is whether AI should be allowed to act.

Mirai Meter is a delegation UI for that boundary.

+--------------------------------------------------------------------+
| Design principles                                                  |
+--------------------------------------------------------------------+

1. Keep the UI stable.

   Personal decisions, business decisions, cloud architecture decisions,
   and embedded AI decisions can all be projected onto the same two axes.

2. Keep judgment traceable.

   When a decision goes wrong, the system should preserve the line of
   reasoning: input, use case, risk axes, data lineage, scoring rules,
   model version, approval path, and execution boundary.

3. Keep AI useful.

   Mirai Meter is not an anti-AI product. It assumes AI can be useful.
   It only separates usefulness from authority.

4. Keep responsibility visible.

   The system should show where human, organizational, or institutional
   confirmation is still required.

5. Keep the final future outside the meter.

   Mirai Meter can show a boundary. It should not become the actor that
   decides the future for the user.

+--------------------------------------------------------------------+
| Example output                                                     |
+--------------------------------------------------------------------+

Request:

    "Please rewrite this apology message."

Output:

    AI contribution:       91%
    Automation permission: 46%

    AI can improve tone, structure, and clarity.
    The user should confirm intent, responsibility, and final delivery.

    Summary:
    "AI can polish the words. The angle of dogeza is user-confirmed."

+--------------------------------------------------------------------+
| Architecture sketch                                                |
+--------------------------------------------------------------------+

Input request
    |
    v
Use case routing
    |
    v
Risk axis extraction
    |
    v
Delegation scoring
    |
    v
Explanation generation
    |
    v
Trace and lineage logging
    |
    v
Meter UI

+--------------------------------------------------------------------+
| Core scoring axes                                                  |
+--------------------------------------------------------------------+

Mirai Meter may consider:

- irreversibility
- external action surface
- interpersonal risk
- financial risk
- legal or compliance risk
- operational responsibility
- verification path
- rollback path
- authority transfer
- purpose-setting risk
- responsibility transfer
- data lineage
- auditability

These axes do not produce a moral verdict.
They produce a delegation boundary.

+--------------------------------------------------------------------+
| Use case registry                                                  |
+--------------------------------------------------------------------+

Mirai Meter should scale by adding use case cards, not by making one
giant prompt.

Each use case card may define:

- domain
- task type
- typical AI contribution
- automation constraints
- risk axes
- explanation template
- expected meter range
- evaluation cases
- source lineage

The UI remains stable as the registry grows.

+--------------------------------------------------------------------+
| Data lineage                                                       |
+--------------------------------------------------------------------+

Because Mirai Meter explains decisions, its own data must be traceable.

Each decision case should preserve:

- source type
- source URL or internal reference
- retrieval time
- license or allowed-use status
- transformation history
- prompt version
- model version
- reviewer status
- label rationale
- evaluation result

Explanation without lineage is not enough.

+--------------------------------------------------------------------+
| Minimal MVP                                                        |
+--------------------------------------------------------------------+

The MVP can be small:

- one input box
- two meters
- one short explanation
- one delegation map
- three demo cases

Recommended demo cases:

1. Meeting notes
2. Apology message
3. Future or career decision

The product should feel light.
The reasoning behind it can be deep.

+--------------------------------------------------------------------+
| Tagline                                                            |
+--------------------------------------------------------------------+

Mirai Meter:
a useful user interface for artificial intelligence.

AI can help.
The meter shows how far it should go.