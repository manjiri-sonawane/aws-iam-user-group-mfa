**Module:** AWS IAM – Identity and Access Management  
**Date Completed:** November 2026  
**Author:** Manjiri Sonawane — [GitHub Profile](https://github.com/manjiri-sonawane)

---

## 📌 What This Project Does

This project covers my hands-on practice with AWS IAM (Identity and Access Management).

I created an IAM user, created an IAM group, added the user to the group, and explored permissions using the AmazonS3ReadOnlyAccess policy. I also learned how to enable MFA for an additional layer of account security.

## 🏗️ Architecture / How It Works

The following shows how IAM user and group permissions are organized.

```text
             AWS IAM
                |
          IAM Group
          s3-read-only
                |
       AmazonS3ReadOnlyAccess
                |
           IAM User
          dev-s3-reader
                |
         S3 Read-Only Access
```

**MFA:** Multi-Factor Authentication adds an extra verification step during sign-in.

## 🛠️ Services & Tools Used

- **AWS:** Identity and Access Management (IAM), Amazon S3
- **IAM Components:** Users, Groups, Policies, MFA
- **Policy:** AmazonS3ReadOnlyAccess
- **Other:** AWS Management Console

## 📋 Steps to Reproduce

1. Sign in to the AWS Management Console.
2. Search for IAM and open the IAM service.
3. Navigate to IAM Users and create a new user.
4. Create an IAM group named `s3-read-only`.
5. Attach the `AmazonS3ReadOnlyAccess` policy to the group.
6. Add the IAM user `dev-s3-reader` to the group.
7. Explore the Security credentials section to learn how to configure MFA.
8. Verify the user's group membership and attached permissions.

## 📸 Screenshot / Proof of Work

Add your own AWS Console screenshots here:

- IAM user creation
- IAM group creation
- Policy attached to the group
- User added to the group
- MFA configuration (if enabled)

Example:

<img width="1425" height="703" alt="Screenshot 2026-11-26 at 10 00 16 PM" src="https://github.com/user-attachments/assets/967ef9a7-f46b-45d4-a791-a7cd1f50d9ce" />



## 💡 What I Learned

- Understood the basics of AWS IAM and why identity management is important.
- Learned how to create IAM users and groups.
- Understood how to attach policies and assign permissions through groups.
- Practiced adding an IAM user to an existing group.
- Learned how MFA improves account security.

## ⚠️ Common Mistakes to Avoid

- Avoid giving unnecessary permissions to IAM users.
- Follow the principle of least privilege.
- Always enable MFA where appropriate.
- Never share AWS access keys, passwords, or secret credentials.
- Never upload sensitive AWS account information in public screenshots.

---

*Built as part of my AWS and DevOps learning journey at [ClouderWay Academy](https://clouderway.com).* 
