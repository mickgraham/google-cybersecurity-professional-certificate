# Activity: Determine appropriate data handling practices

*This activity is based on a fictional scenario.*

**References**

* **data-leak-worksheet.docx:** Data leak worksheet template
* **data-leak-worksheet.docx-exemplar.docx:** Sample solution

## Scenario

You work for an educational technology company that developed an application to help teachers automatically grade assignments. The application handles a wide range of data that it collects from academic institutions, instructors, parents, and students.

Your team was alerted to a data leak of internal business plans on social media. An investigation by the team discovered that an employee accidentally shared those confidential documents with an external business partner. An audit into the leak is underway to determine how similar incidents can be avoided.

A supervisor provided you with information regarding the leak. It appears that the principle of least privilege was not observed by employees at the company during a sales meeting. You have been asked to analyze the situation and find ways to prevent it from happening again.

First, you'll need to evaluate details about the incident. Then, you'll review the controls in place to prevent data leaks. Next, you'll identify ways to improve information privacy at the company. Finally, you'll justify why you think your recommendations will make data handling at the company more secure.

## Determine appropriate data handling practices

**Issue(s):** What factors contributed to the information leak?

* The initial contributing factor is the sales manager deciding not to revoke access once access was no longer needed by the sales team.
* Principle of least privilege was not observed as the sales team member shared a link to the folder instead of only the promotional materials.
* Separation of responsibilities is not present as there is internal-only documents and promotional materials to share with business partners stored in the same folder.

**Review:** What does NIST SP 800-53: AC-6 address?

AC--6 deals with least privilege, which is the sixth category of access controls. It declares that only the minimal access and authorization required to complete a task or function
should be provided to users. It covers automatically revoking access and restricting access based on user role.

**Recommendation(s):** How might the principle of least privilege be improved at the company?

* Revoking access should have been followed by the manager after the meeting where the data was used was completed.
* Restricting access based on user role, which would have been useful in this scenario by restricting internal-only data to employees.

**Justification:** How might these improvements address the issues?

* Following plans for revoking access would mean that the sales team member would not be able to accidentally share entire folder details.
* Restricting access based on user role would mean that even if access was accidentally shared, business partners could not access internal--only data.
