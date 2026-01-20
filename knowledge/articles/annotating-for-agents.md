# Annotating for agents

**Author:** Benji Taylor
**Source:** https://benji.org/annotating
**Date:** January 16, 2026

## Overview

Explores how to provide precise, actionable feedback to AI coding agents on animations and interactions. Rather than describing temporal changes verbally, capture and annotate animations at specific moments to provide agents with exact timing, coordinates, and state information.

## The Problem: Temporal Feedback Gap

Visual feedback tools work well on static snapshots, but animations are temporal. Issues exist in:
- In-between states
- Timing and delays
- Easing curves
- Transition mechanics

**Challenge:** Describing animation problems loses precision. "The button hover feels sluggish" is vague—which part? The delay? Duration? Easing?

## The Solution: Annotation with Captured State

A tool that overlays on localhost allows you to:
- Pause animations at specific moments
- Click on elements mid-transition
- Leave annotated notes
- Capture surrounding context

### Captured Context

The tool captures alongside annotations:
- Timing information
- Coordinates
- File paths
- Animation state
- In-between frame information

### Generate Prompts for Agents

When done annotating, the tool generates a prompt for Claude Code or other agents that includes:
- **What** needs to change
- **When** (precise timing information)
- **Where** (coordinates and elements)
- **How** (state information)

This precision moves feedback from vague observation to actionable specification.

## Key Insight

**"The harder something is to describe, the more helpful it is to just point at it."**

For animations and interactions, showing the exact moment and state is far more effective than describing it verbally. This approach bridges the gap between visual feedback tools and the temporal nature of animations.
