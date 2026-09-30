# Voice-Based-Meal-Verification-
This is a project from our Digital Signal Processing Laboratory course. We built a Meal Verification system with MATLAB using proper algorithms. 
Authors & Project Credits
This project was engineered and submitted by Group 07 (Section C1):

S M Sindid Islam Mahodi (Roll: 2206147) — Lead Author & System Architect
Email: sindidislam101@gmail.com
Samin Zahan Khan (Roll: 2206135)
Syed Ibnul Morshed (Roll: 2206141)
Abdullah Al Rohan (Roll: 2206150)
Academic Supervision:
Department of Electrical and Electronic Engineering
Bangladesh University of Engineering and Technology (BUET), Dhaka-1000, Bangladesh

Executive Summary
In university residence hall dining facilities, meal token theft, manual paper roster overhead, buddy-punching, and coupon duplication cause substantial administrative and financial inefficiencies.

This repository delivers a state-of-the-art Voice-Based Dining Hall Verification and Access Control System combining:

Acoustic Front-end Preprocessing: Rational downsampling (44.1 kHz 
→
 8 kHz), pre-emphasis, Short-Time Energy (STE) + Zero-Crossing Rate (ZCR) voice activity detection, and adaptive spectral noise subtraction.
Content Matching (What was said): 26-channel Mel-filterbank Cepstral Coefficients (MFCC 
c
1
.
.
c
12
 + 
Δ
) with Cepstral Mean and Variance Normalization (CMVN) evaluated against enrolled phrase takes using Dynamic Time Warping (DTW) with Sakoe-Chiba constraint band and cohort normalization.
Voice Biometrics (Who is speaking): 64-mixture Gaussian Mixture Model — Universal Background Model (GMM-UBM) with Maximum A Posteriori (MAP) acoustic adaptation.
Active Anti-Replay Defense: Dynamic randomized 3-digit challenges, acoustic splice detection, and loudspeaker sub-200 Hz spectral energy ratio checks.
Comprehensive Dining Hall Administration: Real-time MATLAB App Designer/uifigure GUI, admin meal window scheduler (Breakfast/Lunch/Dinner), monthly roster entitlements, and immutable single-meal-per-service-session enforcement.
