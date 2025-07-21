# 📂 User Support Document

### 🔹 Issue: User Not Defined

**Troubleshooting Steps:**
1. Search the `users` table in the identity database using the email or username.
2. Check SSO provider logs for recent login attempts.
3. Review onboarding logs or user provisioning service activity in the last 24 hours.
4. Inspect integration sync logs (e.g., from Workday or HRIS if applicable).

**Suggested Actions:**
- Trigger user creation via identity management tool (e.g., Okta, Azure AD).
- Sync user from upstream system.
- Assign default roles and permissions.
- Notify requester once the user is active.

---

### 🔹 Issue: Invalid Login Credentials

**Troubleshooting Steps:**
1. Reproduce the login with test credentials if allowed.
2. Verify user credentials against the authentication provider.
3. Review failed login logs (e.g., `/var/log/auth.log` or SSO audit logs).
4. Check account lockout or password expiry settings.

**Suggested Actions:**
- Initiate password reset link delivery.
- Unlock the user account if locked.
- Educate user on valid username/password format.
- Enable MFA re-registration if necessary.

---

