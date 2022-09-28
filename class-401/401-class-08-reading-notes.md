# Access Control (ACL)

[5 Steps to RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

- What is Role Based Access Control (RBAC) and why do we care?
  - RBAC is the idea of assigning system access to users based on their role within an organization. With tight adherence to access requirements established for each role, access management becomes much easier. With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.
- Describe a Role/Permission heirarchy that you might implement using RBAC.
  - For example, you might have a basic user role, which includes the access any employee would need, such as email and the intranet site. Another role might be a customer service rep, that would have read/write access to the customer database, and a customer database administrator, that would have full control of the customer database.
- What approach might you take to implement RBAC?
  - Inventory your systems, analyze your workforce and create roles, assign people to roles, never make one-off changes, and audit.

[wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)

- If Authentication is “you are who you say you are,” what is Authorization?
  - Authorization is determining what you're allowed access to depending on your role
- Name three primary rules defined for RBAC.
  - Three primary rules are defined for RBAC:
    - Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.
    - Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.
    - Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.
- Describe RBAC to a non-technical friend.
  - Role-based access control is a policy-neutral access-control mechanism defined around roles and privileges. Your role in the company determines what information you have access to.

[RBAC Tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)

- What Are access rights Associated with? The User? or The Role? Explain.
  - The rights are associated with the role. Each use is assigned a role based on there job in the company, each role needs certain recourses that they need access to. The resources you need determine your rights, which are what you are allowed to have access to in the company.
- Access Rights, or Authorization, is activated after a user successfully does what?
  - Users must first authenticate themselves to the system. Then users must be activated into one or more roles, and once they assume one or more roles, based on what those roles give them access to, that what the user or the process runnning on behalf of this user, can access.
- Explain how RBAC might benefit a business.
  - Policy need not be updated when a certain person with a role leaves the organization
  - New employees should be able to activate the desired role
  - Revisiting least privilege
    - User in one role has access to a subset of the files
    - Switch roles to gain acces to other resources
  - SELinux supports RBAC

## Things I want to know more about

- Implementing RBAC into code

[Return home](https://khofstetter94.github.io/reading-notes/)
