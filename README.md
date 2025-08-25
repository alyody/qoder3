# 🏢 LGL HR Portal

A comprehensive Streamlit-based HR management system combining intelligent HR assistance with employee forms management.

## 🚀 Features

### 🤖 HR Assistant
- **Smart Policy Guidance**: AI-powered responses to HR policy questions
- **Leave Balance Tracking**: Real-time leave entitlement calculations
- **Employee Login System**: Personalized experience with employee profiles
- **Interactive Chat Interface**: Natural language policy queries
- **Comprehensive Policy Coverage**: Working hours, leave policies, conduct guidelines

### 📝 Employee Forms Portal
- **Annual Leave Requests**: Date validation and balance tracking
- **Sick Leave Applications**: Medical certificate upload support
- **Emergency Forms**: Quick submission for urgent requests
- **Form Submission Tracking**: JSON-based storage with reference numbers
- **Manager Notification System**: Automatic approval workflow

## 🛠️ Quick Start

### 1. Clone Repository
```bash
git clone <your-repository-url>
cd LGL-HR-Portal
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run Application
```bash
streamlit run app.py
```

### 4. Access Portal
Open your browser to `http://localhost:8501`

## 📋 Requirements

- Python 3.8+
- Streamlit 1.28.0+
- Pandas 1.5.0+

## 🔧 Configuration

### Employee Data
The system includes sample employee profiles in `EMPLOYEE_DATA`:
- **John Doe** (EMP001) - English Teacher, Academic Staff
- **Sarah Smith** (EMP002) - Administrative Assistant, Administration  
- **Ahmed Hassan** (EMP003) - Academic Coordinator, Academic Staff

### Leave Policies
- **Annual Leave**: 20 days (first year) / 22 days (subsequent years)
- **Sick Leave**: 90 days per year
- **Maternity Leave**: 60 days paid + 100 days unpaid
- **Bereavement Leave**: 3-5 days based on relationship

## 🏗️ Project Structure

```
LGL-HR-Portal/
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
├── README.md             # Project documentation
├── .gitignore            # Git ignore rules
└── submissions/          # Form submission storage (auto-created)
    ├── annual_leave_*.json
    ├── sick_leave_*.json
    └── urgent_request_*.json
```

## 🎯 Usage Guide

### HR Assistant Mode
1. **Employee Login**: Select your profile from the sidebar
2. **Quick Topics**: Click buttons for common HR queries
3. **Chat Interface**: Type questions in natural language
4. **Leave Balance**: Check remaining days with "my leave balance"

### Employee Forms Mode
1. **Navigate**: Use sidebar to switch to "Employee Forms"
2. **Select Form**: Choose from available form types
3. **Fill Details**: Complete required fields with validation
4. **Submit**: Receive confirmation with reference number

### Available Forms
- 🏖️ **Annual Leave Request** - Vacation time off
- 🏥 **Sick Leave Request** - Medical leave with certificate upload
- 👶 **Maternity/Parental Leave** - Family leave (quick request)
- 🕊️ **Bereavement Leave** - Compassionate leave (quick request)
- 📋 **Resignation Letter** - Employment termination (quick request)
- ⭐ **Performance Review Request** - Additional evaluations (quick request)
- 🎓 **Training Request** - Professional development (quick request)
- 📢 **Grievance/Complaint** - Workplace issues (quick request)

## 🌐 Deployment

### Streamlit Cloud Deployment

1. **Create GitHub Repository**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin <your-github-repo-url>
   git push -u origin main
   ```

2. **Deploy to Streamlit Cloud**
   - Visit [streamlit.io](https://streamlit.io)
   - Sign in with GitHub
   - Click "New app"
   - Select your repository
   - Set main file: `app.py`
   - Click "Deploy"

3. **Configuration**
   - App will be available at: `https://<app-name>.streamlit.app`
   - Automatic updates on GitHub pushes
   - Free tier supports unlimited public apps

### Alternative Deployment Options

- **Heroku**: Use `setup.sh` and `Procfile` for Heroku deployment
- **AWS/Azure**: Docker containerization for cloud platforms
- **Local Network**: Deploy on internal servers for enterprise use

## 🔒 Security & Privacy

- **Employee Data**: Stored locally in application memory
- **Form Submissions**: JSON files saved to local `submissions/` directory
- **No External Dependencies**: No external database or API calls required
- **Data Privacy**: No sensitive data transmitted externally

## 📊 Data Management

### Form Storage
- **Format**: JSON files with timestamp
- **Location**: `submissions/` directory
- **Naming**: `{form_type}_{YYYYMMDD_HHMMSS}.json`
- **Content**: Complete form data with employee information

### Leave Calculations
- Automatic entitlement calculations based on service years
- Real-time balance updates
- Policy compliance checking

## 🎨 Customization

### Branding
- **Colors**: LGL blue gradient theme
- **Logo**: Update in header section
- **Company Info**: Modify footer and contact details

### Adding Employees
```python
'new_employee_key': {
    'name': 'Employee Name',
    'department': 'Department',
    'employee_id': 'EMP###',
    'approval_manager': 'Manager Name',
    # ... other fields
}
```

### Policy Updates
Update `HANDBOOK_DATA` dictionary with new policies and keywords.

## 🐛 Troubleshooting

### Common Issues
1. **Port Already in Use**: Use `streamlit run app.py --server.port 8502`
2. **Module Not Found**: Ensure all dependencies installed with `pip install -r requirements.txt`
3. **Form Not Submitting**: Check required fields and validation

### Browser Issues
- **Clear Cache**: Hard refresh with Ctrl+F5
- **Incognito Mode**: Test in private browsing
- **Different Browser**: Try Chrome, Firefox, or Edge

## 🔄 Updates & Maintenance

### Regular Tasks
- Update employee database as needed
- Review and archive form submissions
- Update policy information in handbook data
- Monitor system performance and usage

### Version Control
- Tag releases for major updates
- Maintain changelog for deployments
- Backup form submissions before updates

## 📞 Support

### Technical Support
- **Repository Issues**: Use GitHub Issues tab
- **Email**: lgldubai@gmail.com
- **Internal**: Contact IT Department

### User Support
- **HR Queries**: Use the built-in HR Assistant
- **Form Issues**: Submit grievance form
- **Training**: Contact HR for user training

## 📈 Future Enhancements

### Planned Features
- Database integration for scalability
- Email notification system
- Digital signature support
- Advanced reporting dashboard
- Mobile app development
- Integration with existing HRIS

### Community Contributions
- Fork the repository
- Create feature branches
- Submit pull requests
- Follow coding standards

## 📄 License

This project is proprietary software developed for LGL internal use.

## 🏆 Acknowledgments

- Built with Streamlit framework
- Designed for LGL HR operations
- Developed following LGL company policies

---

**© 2025 LGL. All rights reserved.**

For the latest updates and documentation, visit the project repository.