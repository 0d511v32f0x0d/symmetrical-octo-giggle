# Credentials

<style>
.user-card {
  background: linear-gradient(145deg, #ffffff, #f5f7fa);
  border-radius: 20px;
  padding: 2rem;
  margin: 2rem 0;
  box-shadow: 0 15px 35px rgba(0,0,0,0.1);
  transition: all 0.3s ease;
  border: 1px solid rgba(255,255,255,0.2);
  backdrop-filter: blur(10px);
}

.user-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 20px 40px rgba(0,0,0,0.15);
}

.user-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1.5rem;
  padding-bottom: 1rem;
  border-bottom: 2px solid #eef2f7;
}

.cred-title {
  font-size: 1.75rem;
  font-weight: 700;
  color: #1a365d;
  margin: 0;
}

.role-badge {
  padding: 0.5rem 1.5rem;
  border-radius: 9999px;
  font-size: 0.875rem;
  font-weight: 600;
  letter-spacing: 0.5px;
  text-transform: uppercase;
}

.role-badge.base {
  background: linear-gradient(135deg, #e6f3ff, #dbeafe);
  color: #2563eb;
}

.role-badge.admin {
  background: linear-gradient(135deg, #f3e8ff, #e9d5ff);
  color: #7e22ce;
}

.details-content {
  margin-top: 1.5rem;
  padding: 1.5rem;
  background: #f8fafc;
  border-radius: 12px;
  border: 1px solid #e2e8f0;
}

.detail-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.75rem 0;
  border-bottom: 1px solid #e2e8f0;
}

.detail-item:last-child {
  border-bottom: none;
}

.detail-label {
  color: #64748b;
  font-weight: 500;
  font-size: 0.95rem;
  min-width: 120px;
}

.detail-value {
  color: #1e293b;
  font-weight: 600;
  font-size: 1rem;
  flex-grow: 1;
  text-align: right;
  margin-right: 0.5rem;
}

.copy-button {
  background: #f1f5f9;
  border: 1px solid #e2e8f0;
  padding: 0.25rem 0.75rem;
  border-radius: 6px;
  font-size: 0.75rem;
  color: #64748b;
  cursor: pointer;
  transition: all 0.2s ease;
  min-width: 60px;
}

.copy-button:hover {
  background: #e2e8f0;
  color: #1e293b;
  transform: translateY(-1px);
}

.department-section {
  margin: 3rem 0;
}

.department-title {
  font-size: 2.5rem;
  color: #1a365d;
  margin-bottom: 2rem;
  padding-bottom: 0.5rem;
  border-bottom: 3px solid #e2e8f0;
  text-align: center;
  font-weight: 700;
}

.user-type-title {
  font-size: 1.75rem;
  color: #334155;
  margin: 2rem 0 1rem;
  text-align: center;
  font-weight: 600;
}

.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
  margin: 1rem 0;
  padding: 1rem;
}
</style>

<script>
function copyToClipboard(text) {
  navigator.clipboard.writeText(text);
}
</script>

<!-- ## Department Structure
Each department has:
- Base Users (role_id: 3)
- Admin Users (role_id: 2) -->

## Sales Department


<div class="grid-container">
  <div class="user-card">
    <div class="user-header">
      <h3 class="cred-title">Test Cred 1</h3>
      <span class="role-badge base">Base User</span>
    </div>
    <div class="details-content">
      <div class="detail-item">
        <span class="detail-label">Username</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">SalesUser1</span>
          <button class="copy-button" onclick="copyToClipboard('SalesUser1')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Password</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Root@123</span>
          <button class="copy-button" onclick="copyToClipboard('Root@123')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Email</span>
        <span class="detail-value">salesuser1@example.com</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Employee ID</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">SA101</span>
          <button class="copy-button" onclick="copyToClipboard('SA101')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Contact</span>
        <span class="detail-value">09111111111</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Department</span>
        <span class="detail-value">Sales</span>
      </div>
    </div>
  </div>

  <div class="user-card">
    <div class="user-header">
      <h3 class="cred-title">Test Cred 2</h3>
      <span class="role-badge base">Base User</span>
    </div>
    <div class="details-content">
      <div class="detail-item">
        <span class="detail-label">Username</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">SalesUser2</span>
          <button class="copy-button" onclick="copyToClipboard('SalesUser2')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Password</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Root@123</span>
          <button class="copy-button" onclick="copyToClipboard('Root@123')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Email</span>
        <span class="detail-value">salesuser2@example.com</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Employee ID</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">SA102</span>
          <button class="copy-button" onclick="copyToClipboard('SA102')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Contact</span>
        <span class="detail-value">09111111112</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Department</span>
        <span class="detail-value">Sales</span>
      </div>
    </div>
  </div>
</div>

### Admin Users

<div class="grid-container">
  <div class="user-card">
    <div class="user-header">
      <h3 class="cred-title">Test Cred 3</h3>
      <span class="role-badge admin">Admin</span>
    </div>
    <div class="details-content">
      <div class="detail-item">
        <span class="detail-label">Username</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Sales_Admin1</span>
          <button class="copy-button" onclick="copyToClipboard('Sales_Admin1')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Password</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Root@123</span>
          <button class="copy-button" onclick="copyToClipboard('Root@123')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Email</span>
        <span class="detail-value">salesadmin1@example.com</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Employee ID</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">SA201</span>
          <button class="copy-button" onclick="copyToClipboard('SA201')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Contact</span>
        <span class="detail-value">09111111121</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Department</span>
        <span class="detail-value">Sales</span>
      </div>
    </div>
  </div>

  <div class="user-card">
    <div class="user-header">
      <h3 class="cred-title">Test Cred 4</h3>
      <span class="role-badge admin">Admin</span>
    </div>
    <div class="details-content">
      <div class="detail-item">
        <span class="detail-label">Username</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Sales_Admin2</span>
          <button class="copy-button" onclick="copyToClipboard('Sales_Admin2')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Password</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Root@123</span>
          <button class="copy-button" onclick="copyToClipboard('Root@123')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Email</span>
        <span class="detail-value">salesadmin2@example.com</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Employee ID</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">SA202</span>
          <button class="copy-button" onclick="copyToClipboard('SA202')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Contact</span>
        <span class="detail-value">09111111122</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Department</span>
        <span class="detail-value">Sales</span>
      </div>
    </div>
  </div>
</div>

## Technical Department


<div class="grid-container">
  <div class="user-card">
    <div class="user-header">
      <h3 class="cred-title">Test Cred 5</h3>
      <span class="role-badge base">Base User</span>
    </div>
    <div class="details-content">
      <div class="detail-item">
        <span class="detail-label">Username</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">TechUser</span>
          <button class="copy-button" onclick="copyToClipboard('TechUser')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Password</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Root@123</span>
          <button class="copy-button" onclick="copyToClipboard('Root@123')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Email</span>
        <span class="detail-value">techuser@example.com</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Employee ID</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">CU111</span>
          <button class="copy-button" onclick="copyToClipboard('CU111')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Contact</span>
        <span class="detail-value">09876543210</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Department</span>
        <span class="detail-value">Technical</span>
      </div>
    </div>
  </div>

  <div class="user-card">
    <div class="user-header">
      <h3 class="cred-title">Test Cred 6</h3>
      <span class="role-badge base">Base User</span>
    </div>
    <div class="details-content">
      <div class="detail-item">
        <span class="detail-label">Username</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">TechUser2</span>
          <button class="copy-button" onclick="copyToClipboard('TechUser2')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Password</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Root@123</span>
          <button class="copy-button" onclick="copyToClipboard('Root@123')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Email</span>
        <span class="detail-value">techuser2@example.com</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Employee ID</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">CU112</span>
          <button class="copy-button" onclick="copyToClipboard('CU112')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Contact</span>
        <span class="detail-value">09876543211</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Department</span>
        <span class="detail-value">Technical</span>
      </div>
    </div>
  </div>
</div>

### Admin Users

<div class="grid-container">
  <div class="user-card">
    <div class="user-header">
      <h3 class="cred-title">Test Cred 7</h3>
      <span class="role-badge admin">Admin</span>
    </div>
    <div class="details-content">
      <div class="detail-item">
        <span class="detail-label">Username</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Tech_Admin</span>
          <button class="copy-button" onclick="copyToClipboard('Tech_Admin')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Password</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Root@123</span>
          <button class="copy-button" onclick="copyToClipboard('Root@123')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Email</span>
        <span class="detail-value">techadmin@example.com</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Employee ID</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">CU222</span>
          <button class="copy-button" onclick="copyToClipboard('CU222')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Contact</span>
        <span class="detail-value">09876543210</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Department</span>
        <span class="detail-value">Technical</span>
      </div>
    </div>
  </div>

  <div class="user-card">
    <div class="user-header">
      <h3 class="cred-title">Test Cred 8</h3>
      <span class="role-badge admin">Admin</span>
    </div>
    <div class="details-content">
      <div class="detail-item">
        <span class="detail-label">Username</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Tech_Admin2</span>
          <button class="copy-button" onclick="copyToClipboard('Tech_Admin2')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Password</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">Root@123</span>
          <button class="copy-button" onclick="copyToClipboard('Root@123')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Email</span>
        <span class="detail-value">techadmin2@example.com</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Employee ID</span>
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="detail-value">CU223</span>
          <button class="copy-button" onclick="copyToClipboard('CU223')">Copy</button>
        </div>
      </div>
      <div class="detail-item">
        <span class="detail-label">Contact</span>
        <span class="detail-value">09876543212</span>
      </div>
      <div class="detail-item">
        <span class="detail-label">Department</span>
        <span class="detail-value">Technical</span>
      </div>
    </div>
  </div>
</div>

> **Note**: All users have the default password `Root@123`. Please ensure to change passwords after first login.