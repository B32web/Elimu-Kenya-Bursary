# Elimu Kenya
Pages: index.html (website) -> apply.html (details + submit) -> pay.html (processing fee).
Fees by band: 5=KSh 100, 4=150, 3=200, 2=250, 1=300 (shown only on the last review step and payment page).
Setup: 1) Run schema.sql in Supabase SQL Editor. 2) Put your Project URL and anon key in config.js. 3) Push the folder to Vercel (no build step).
Verifying payments: check the M-Pesa SMS code in the payments table, then set applications.status = 'verified'. The student's pay page then shows the success notice.
Leaving config.js blank runs a local preview mode that auto-confirms payment. Never deploy that way.
