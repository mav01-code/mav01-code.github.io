# Amazon SDE-1 Intern (6 months) - off campus hiring

## Details

Stipend - 1.3 lakh/month

Location - Bangalore, KA

Duration - 6 months

## Rounds

1. Online Assessment (Coding + Repo based question with AI assistant + Workstyle Assessment)
2. Technical Round - 1

## Timeline

1. 03/08/2026 - Application submitted on Amazon careers and completed OA
2. 19/10/2026 (01:48 PM)- Got a mail saying I'm shortlisted for interview and will be receiving schedule soon
3. 19/10/2026 (06:47 PM) - Interview schedule for round 1
4. 21/10/2026 (10:00 - 11:00 AM) - Round -1 interview

## Experience

### OA

Consists 1 coding question, repository based debugging using AI assistant, workstyle assessment. Passed all test cases for coding question. Repo based - was able to pass 2/6 testcases and completed workstyle assessment.

### Round - 1 (Technical interview)

Interviewer is Manvendra Chauhan, SDE-2 working in Amazon payments. Interviewer gave intro and asked me to give mine. Later, we moved on to coding question (DSA).

#### Question:

You are given an array of signals where each signal represents the strength of signal at i. You are also given a value k which represents stable strength.

Goal is to find the maximum length of the window [l, r] where difference of max and min of that window is atmost k.

#### Algorithm: Variable sliding window

#### Solution I gave:

```Python
def func(signals, k):
  q = deque()
  res = 0
  m, M = float('inf'), float('-inf')
  l = 0
  for r in range(len(signals)):
    q.append(signals[r])
    if signals[r] < m:
      m = signals[r]
    if signals[r] > M:
      M = signals[r]
    if M - m > k:
      while True:
        top = q.popleft()
        if top == m or top == M:
          break
    res = max(res, len(q))
```


#### Time Complexity -> O(n^2)

#### Space Complexity -> O(n)

#### LP Questions

1. Since you said you're doing an internship, you must have been assigned a project. What are the tradeoffs, feedback and how did you make sure to complete it within deadline?
2. What is the feedback that you received?

#### My questions

1. Will I have round 2 after this?
2. What will interns work on?
3. For an intern to be converted to full time, what are the factors affecting?
