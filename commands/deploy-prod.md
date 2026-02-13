---
name: deploy-prod
description: Deploy application to production environment
---

# Production Deployment Command

## Overview
Safely deploy the application to the production environment with validation checks and rollback capability.

## Execution Steps

1. **Pre-deployment Checks**
   - Verify all tests pass
   - Check code coverage meets minimum threshold
   - Validate no uncommitted changes exist
   - Confirm branch is synced with main

2. **Build Phase**
   - Run build process
   - Verify build artifacts are created successfully
   - Run final integration tests on built artifacts

3. **Deployment Phase**
   - Create a backup of current production state
   - Deploy new version to staging first
   - Run smoke tests on staging
   - Deploy to production environment

4. **Post-deployment Verification**
   - Verify health check endpoints respond correctly
   - Check error logs for anomalies
   - Monitor performance metrics
   - Send deployment notification to team

## Rollback
If any step fails, immediately:
1. Stop deployment process
2. Revert to previous known-good state
3. Notify team and incident responders
4. Document failure details

## Safety
- Always deploy to staging first
- Maintain database backups
- Keep previous version running during transition (blue-green deploy)
