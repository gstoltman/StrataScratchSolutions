SELECT employee_title, sex, AVG(salary + sumbonus) as average
FROM sf_employee a
INNER JOIN (SELECT worker_ref_id, SUM(bonus) AS sumbonus
FROM sf_bonus
GROUP BY worker_ref_id) b
ON a.id = b.worker_ref_id
GROUP BY employee_title, sex
