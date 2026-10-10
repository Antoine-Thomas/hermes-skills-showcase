# Use-cases

## Video Automation

### Talking Head Video Creation
- **Scenario**: Create a video presenter from a single photo and audio recording
- **Workflow**: `hermes run liveportrait-pipeline --source photo.jpg --audio recording.wav`
- **Result**: Animated talking head video at 11.1x realtime speed
- **Use case**: Educational content, tutorials, presentations without appearing on camera

### Video Assembly
- **Scenario**: Combine multiple media elements into a final video
- **Workflow**: `hermes run video-youtube-assembly --music track.mp3 --logo overlay.png`
- **Result**: Synced video with audio, title card, and logo overlay
- **Use case**: YouTube content creation, marketing videos

## System Optimization

### OmniRoute Auto-Update
- **Scenario**: Keep AI model selection optimized for cost vs performance
- **Workflow**: `hermes run omniroute-auto-update`
- **Result**: Automatically adds new free AI models, updates config, notifies Telegram
- **Use case**: Reduce API costs while maintaining quality

### Windows Optimization
- **Scenario**: Clean and optimize a Windows system for media production
- **Workflow**: `hermes run windows-optimization --clean-temp --optimize-tasks`
- **Result**: Freed disk space, optimized task scheduling, improved performance
- **Use case**: Maintain production workstations

## WordPress Automation

### Local Site Setup
- **Scenario**: Quickly set up a new WordPress development site
- **Workflow**: `hermes run local-flywheel-setup --site-name "client-site" --php-version "8.2"`
- **Result**: Fully configured WordPress on Local by Flywheel in minutes
- **Use case**: Client demos, development environments

### Backup and Restore
- **Scenario**: Protect WordPress sites against data loss
- **Workflow**: `hermes run wordpress-backup-restore --action backup --site-name "my-site"`
- **Result**: Complete archive with files and database, stored locally
- **Use case**: Disaster recovery, before major changes

### Remote Deployment
- **Scenario**: Deploy a local WordPress site to a production server
- **Workflow**: `hermes run wordpress-deployment --target ftp --host "ftp.example.com" --path "/www"`
- **Result**: Files uploaded, database synced, URLs updated for production
- **Use case**: Launch sites from local to live environment