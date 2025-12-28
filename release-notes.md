---
layout: page
title: Release Notes
permalink: /release-notes/
---

Stay updated with the latest improvements, features, and fixes in NutriComposer.

---

## Version 2.0.35 (December 27, 2025)
### App Store Release
- Initial App Store submission
- Added required privacy usage descriptions for HealthKit and Microphone access
- Disabled default API key for public release
- Minor bug fixes and performance improvements

## Version 2.0.34 (December 27, 2025)
### AI Assistant Fixes and UX Improvements
- Fixed AI intent classification: "What should I eat for dinner?" now correctly suggests foods instead of adding them
- Fixed AI protein reporting: "How much protein have I eaten?" now shows accurate gram values
- Added key nutrient values (protein, carbs, fat, etc.) to AI context for accurate intake queries
- Improved question detection: Questions with "?" or question words are now prioritized before action keywords
- Removed ambiguous "for breakfast/lunch/dinner" from add-food triggers (could be questions or logs)
- My Targets: "Save Profile & Apply Targets" button now provides visual and haptic feedback
- Save button shows checkmark icon and "Targets Saved!" confirmation for 2 seconds

---

## Version 2.0.33 (December 26, 2025)
### Dark Theme and UI Polish
- Implemented consistent dark theme across Add Food and Compose views
- Added custom colors: appInputField (#404040), appBadge (#606060), appTabInactive (#505050)
- Updated food source badges (FNDDS, USDA, OFF) with light gray background for visibility
- Changed active tab button color to orange with inactive tabs using dark gray
- Centered all buttons in Settings sub-views (My Targets, USDA API Key, Data Management)
- Moved "Clear API Key" to its own section for better visual separation
- All list rows now use consistent dark background

---

## Version 2.0.31 (December 25, 2025)
### Unit Tests and UI Fixes
- Added unit test target with 40+ test cases covering core components
- Tests cover: Balancer, USDAService, OpenFoodFacts parsing, DataStore, Nutrient models
- Fixed: Delete Entry button styling (gray background, black text/icon)
- Fixed: Favorites star icon now uses primary color (black) instead of yellow
- Fixed: Create Food nutrition tabs now use grid layout instead of horizontal scroll
- Fixed: All nutrition category tabs now use consistent blue color

---

## Version 2.0.30 (December 25, 2025)
### Code Refactoring
- Extracted AddFoodSheet component with nutrient progress display
- Extracted CreateFoodSheet, EditFoodAsCustomSheet, EditCustomFoodSheet, EditAndAddToFavoritesSheet to CustomFoodSheets.swift
- FoodSearchView reduced from ~1950 to 740 lines for better maintainability

---

## Version 2.0.29 (December 25, 2025)
### Swift 6 Compatibility and Refactoring
- Fixed Swift 6 concurrency errors by adding Sendable conformance to data types
- Extracted FoodRow component to separate file for better code organization
- Moved AppSettings and WaterData structs to file scope for Swift 6 compatibility

---

## Version 2.0.28 (December 25, 2025)
### Error Handling and Bug Fixes
- Added proper error logging for all data persistence operations
- All file writes now use atomic operations for data safety
- Fixed: Dashboard now loads data correctly on app startup (was requiring pull-to-refresh)

---

## Version 2.0.27 (December 25, 2025)
### Performance Optimizations
- Background thread I/O: All JSON file loading now happens on background threads in parallel
- Reduced view dependency scope: FocusNutrientsCardView and WaterTrackingSectionView now receive specific data instead of full DataStore
- Renamed caloriesPieChartCard to caloriesSummaryCard for accuracy
- Optimized dashboard rendering
- Reduced memory usage

---

## Version 2.0.26 (December 25, 2025)
### Focus Nutrients Composition View
- New composition view for Focus Nutrients
- Visual breakdown of nutrient sources
- Detailed analysis of where nutrients come from
- Enhanced nutrient tracking insights

---

## Version 2.0.25 (December 24, 2025)
### Contributing Foods Feature
- New feature to contribute foods to databases
- Help improve food data for the community
- Submit nutritional information for missing foods
- Community-driven database improvements

---

## Version 2.0.24 (December 24, 2025)
### Food Diary Accessibility and UI Refinements
- Major accessibility improvements for VoiceOver users
- UI refinements and visual polish
- Better font sizing and contrast
- Enhanced usability for all users

---

## Version 2.0.23 (December 23, 2025)
### Dashboard Compact UI Redesign
- New compact dashboard design
- More information in less space
- Improved visual hierarchy
- Better organization of dashboard elements

---

## Version 2.0.22 (December 23, 2025)
### Apple Health Integration Fix
- Fixed Apple Health sync issues
- Resolved calorie and step count reading bugs
- Improved HealthKit integration reliability
- Fixed permission handling edge cases

---

## Version 2.0.21 (December 23, 2025)
### Accessibility Color Improvements
- Enhanced color contrast for better accessibility
- Improved visibility for color-blind users
- Better adherence to WCAG guidelines
- More readable text and UI elements

---

## Version 2.0.20 (December 22, 2025)
### AI Intent Classification Fix
- Fixed AI intent classification accuracy
- Better understanding of user commands
- Improved response relevance
- Enhanced natural language processing

---

## Version 2.0.19 (December 22, 2025)
### Dashboard Refactoring for Performance
- Complete dashboard code refactoring
- Improved architecture and modularity
- Better performance and responsiveness
- Enhanced maintainability

---

## Version 2.0.18 (December 22, 2025)
### Dashboard Energy Summary Redesign
- Redesigned energy summary widget
- New visual representation of calories
- Better tracking of energy intake vs. burn
- Improved at-a-glance information

---

## Version 2.0.17 (December 22, 2025)
### UI Polish and Bug Fixes
- General UI polish and refinements
- Fixed various minor bugs
- Visual consistency improvements
- Performance optimizations

---

## Version 2.0.16 (December 21, 2025)
### Settings Refactoring and Bug Fixes
- Complete settings screen refactoring
- Better organization of settings options
- Improved navigation and usability
- Enhanced settings management

---

## Version 2.0.15 (December 21, 2025)
### Nutrient Progress Bars in Food Details
- New visual progress bars for nutrients
- Color-coded progress indicators
- Easy tracking of daily goals
- Enhanced dashboard visualizations

---

## Version 2.0.14 (December 20, 2025)
### Vitamin D Unit Fix and Accessibility
- Fixed Vitamin D unit display (IU to mcg)
- Corrected nutrient calculations
- Accurate RDA tracking
- Resolved unit conversion issues

---

## Version 2.0.13 (December 20, 2025)
### Branded Database and Data Source Picker
- Added Branded Foods database (296K products)
- Expanded food search options
- Better coverage of packaged foods
- No API key required

---

## Version 2.0.12 (December 20, 2025)
### FNDDS Database Integration
- Integrated FNDDS database (5,400+ foods)
- Added survey foods and common recipes
- More comprehensive food search
- Enhanced database options

---

## Version 2.0.11 (December 19, 2025)
### Auto-Calculate Targets
- New auto-calculate feature for nutrient targets
- Based on age, gender, weight, and activity level
- Personalized recommendations
- Customizable adjustments

---

## Version 2.0.10 (December 19, 2025)
### Documentation Update &amp; Bug Fixes
- Improved in-app documentation
- Better help and tutorial content
- Enhanced user guidance
- More comprehensive FAQs

---

## Version 2.0.9 (December 19, 2025)
### UI Updates and Rebranding
- Major UI refresh with new design language
- Rebranding to NutriComposer
- Modern, clean interface
- Better user experience

---

## Version 2.0.8 (December 18, 2025)
### Favorites Nutrient Fix
- Fixed nutrient calculations for favorite foods
- Corrected serving size handling
- Accurate nutrient totals
- Improved favorites functionality

---

## Version 2.0.7 (December 18, 2025)
### Voice Create Custom Food
- Voice command to create custom foods
- Natural language food creation
- Example: "Create salmon with 166 cal, 26g protein"
- AI-powered nutrient parsing

---

## Version 2.0.6 (December 18, 2025)
### Import Data Bug Fix
- Fixed CSV import functionality
- Resolved data parsing issues
- Improved import reliability
- Better error handling for imports

---

## Version 2.0.5 (December 17, 2025)
### Voice Food Logging
- Voice commands to log foods
- Natural language food entry
- Example: "Add 100g banana to breakfast"
- AI-powered meal logging

---

## Version 2.0.3 (December 16, 2025)
### Performance Optimization
- Significant app performance improvements
- Faster loading and navigation
- Optimized data processing
- Reduced battery usage

---

## Version 2.0.2 (December 16, 2025)
### Edit Custom Foods and Bug Fixes
- New feature to edit custom foods
- Update nutritional information anytime
- Modify serving sizes and nutrients
- Enhanced custom food management

---

## Version 2.0.1 (December 15, 2025)
### Voice Selection
- Added voice selection for AI Assistant
- Multiple voice options
- Improved voice chat experience
- Enhanced voice customization

---

## Version 2.0.0 (December 15, 2025)
### AI Assistant
- Major Release: AI Assistant powered by Apple Foundation Framework LLM
- 100% On-Device: Complete privacy - no data sent to external servers
- Text and voice chat capabilities
- Context-aware nutritional guidance
- Voice food logging and custom food creation
- Siri integration with 9 voice commands
- Natural language interactions
- Intelligent nutrient analysis and recommendations

---

*Thank you for using NutriComposer! We're constantly working to improve your nutrition tracking experience.*
