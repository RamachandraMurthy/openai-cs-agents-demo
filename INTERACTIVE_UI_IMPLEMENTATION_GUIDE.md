# Interactive UI Components in Agent-Based Applications
## Implementation Guide

### Table of Contents
1. [Overview](#overview)
2. [Architecture Pattern](#architecture-pattern)
3. [Backend Implementation](#backend-implementation)
4. [API Middleware](#api-middleware)
5. [Frontend Implementation](#frontend-implementation)
6. [Component Examples](#component-examples)
7. [Best Practices](#best-practices)
8. [Advanced Patterns](#advanced-patterns)
9. [Testing & Debugging](#testing--debugging)
10. [Security Considerations](#security-considerations)

---

## Overview

This guide describes how to implement interactive UI components within agent-based chat applications using a **signal-based communication pattern**. This pattern allows AI agents to dynamically trigger rich, interactive user interface elements within the chat flow, transforming simple text conversations into sophisticated, app-like experiences.

## 🔥 Live Examples & References

Before diving into implementation, explore these live examples of signal-based interactive components in production systems:

### **Interactive Demo Environments**
- **[Slack Block Kit Builder](https://api.slack.com/block-kit/building)** - Live interactive demo with buttons, forms, modals, and date pickers
- **[Microsoft Adaptive Cards Designer](https://adaptivecards.io/designer/)** - Real-time adaptive card builder with live previews
- **[Block Kit Visual Builder](https://app.slack.com/block-kit-builder)** - Drag-and-drop prototyping for interactive chat components

### **Production Implementations**
- **Slack Apps**: Expense approval workflows, incident management, team polls
- **Microsoft Teams**: Security incident response, survey forms, notification cards
- **Discord Bots**: Interactive slash commands, role management, server configuration
- **GitHub**: Pull request reviews, issue management, deployment approvals

### **Documentation & Tutorials**
- **[Slack Block Kit Documentation](https://api.slack.com/block-kit)** - Comprehensive guide to interactive chat components
- **[Microsoft Teams Adaptive Cards](https://learn.microsoft.com/en-us/microsoftteams/platform/task-modules-and-cards/cards/design-effective-cards)** - Design patterns for interactive cards
- **[Interactive Notification Tutorial](https://api.slack.com/tutorials/tracks/actionable-notifications)** - Step-by-step guide to building interactive messages

### **Key Learning Points from Live Examples**
1. **Signal Detection Pattern**: All platforms use marker/signal detection to trigger UI components
2. **Component Variety**: Buttons, forms, maps, calendars, file uploads, image galleries
3. **State Management**: Components maintain state across interactions
4. **Response Handling**: User interactions seamlessly continue chat conversations
5. **Professional UX**: Enterprise-grade implementations show production best practices

### What You Can Create

The signal-based pattern enables you to build virtually any interactive component imaginable. Here are comprehensive categories with specific examples:

#### 🗺️ **Maps & Location Components**
- **Interactive Maps**: Flight routes, delivery tracking, store locators
- **Floor Plans**: Hotel layouts, office maps, venue seating charts
- **Geographic Visualizations**: Weather maps, territory coverage, real estate listings
- **Navigation Aids**: Step-by-step directions with interactive waypoints
- **Location Pickers**: Address selection, geofencing setup, delivery zones

#### 📅 **Date, Time & Scheduling Components**
- **Calendar Widgets**: Appointment booking, availability checking, event planning
- **Date Range Pickers**: Vacation booking, report generation, subscription management
- **Time Slot Selectors**: Meeting scheduling, service appointments, reservation systems
- **Timeline Visualizations**: Project milestones, historical events, progress tracking
- **Recurring Event Builders**: Subscription setup, recurring meetings, reminder schedules

#### 📊 **Data Visualization & Analytics**
- **Interactive Charts**: Sales dashboards, performance metrics, trend analysis
- **Real-time Graphs**: Live monitoring, stock prices, sensor data streams
- **Comparison Tables**: Product features, pricing plans, specification grids
- **Progress Indicators**: Project status, goal tracking, skill development
- **Heat Maps**: Activity patterns, geographic data, performance matrices

#### 🛒 **E-commerce & Shopping**
- **Product Configurators**: Custom PC builds, car options, furniture customization
- **Size Guides**: Clothing fit tools, dimension calculators, compatibility checkers
- **Comparison Tools**: Side-by-side product analysis, feature matrices
- **Wishlist Managers**: Save items, share collections, track prices
- **Inventory Browsers**: Stock levels, variant selection, availability checking

#### 📋 **Forms & Data Collection**
- **Multi-step Wizards**: Onboarding flows, application processes, setup guides
- **Dynamic Forms**: Conditional fields, real-time validation, auto-completion
- **Survey Tools**: Feedback collection, market research, satisfaction scoring
- **Document Builders**: Resume creators, contract generators, report templates
- **Data Import/Export**: File uploaders, format converters, bulk operations

#### 🎮 **Interactive Media & Content**
- **Image Galleries**: Photo browsing, portfolio viewers, before/after comparisons
- **Video Players**: Training content, product demos, tutorial sequences
- **Audio Controls**: Podcast players, music selection, voice message playback
- **Document Viewers**: PDF readers, slide presentations, manual browsers
- **3D Visualizations**: Product models, architectural walkthroughs, scientific data

#### ✈️ **Travel & Transportation**
- **Seat Selection**: Airlines, theaters, events, restaurants
- **Route Planning**: Multi-stop itineraries, alternative paths, cost comparisons
- **Booking Flows**: Hotels, flights, rental cars, activities
- **Check-in Systems**: Mobile boarding passes, room keys, event tickets
- **Tracking Displays**: Package delivery, flight status, vehicle location

#### 🏥 **Healthcare & Wellness**
- **Appointment Schedulers**: Doctor visits, lab tests, therapy sessions
- **Symptom Checkers**: Interactive body diagrams, severity assessments
- **Medication Managers**: Pill schedules, interaction checkers, refill reminders
- **Health Trackers**: Fitness goals, diet logging, mood monitoring
- **Treatment Plans**: Progress visualization, milestone tracking, compliance monitoring

#### 🏦 **Financial Services**
- **Account Dashboards**: Balance views, transaction history, spending analysis
- **Investment Tools**: Portfolio allocation, risk assessment, performance tracking
- **Loan Calculators**: Payment schedules, interest comparisons, affordability tools
- **Budget Planners**: Expense categorization, savings goals, financial forecasting
- **Transaction Flows**: Payment processing, transfer setup, bill pay automation

#### 🏢 **Business & Productivity**
- **Project Managers**: Task boards, Gantt charts, resource allocation
- **Team Collaboration**: Shared workspaces, file sharing, comment systems
- **CRM Tools**: Contact management, pipeline tracking, lead scoring
- **Inventory Systems**: Stock tracking, reorder points, supplier management
- **Analytics Dashboards**: KPI monitoring, report generation, trend analysis

#### 🎓 **Education & Training**
- **Course Browsers**: Curriculum exploration, prerequisite tracking, progress monitoring
- **Interactive Lessons**: Quizzes, simulations, hands-on exercises
- **Assessment Tools**: Test builders, grading systems, performance analytics
- **Learning Paths**: Skill development, certification tracking, goal setting
- **Study Aids**: Flashcards, note-taking, collaboration tools

#### 🎨 **Creative & Design**
- **Color Pickers**: Theme builders, brand management, accessibility checking
- **Layout Builders**: Website creators, newsletter design, presentation tools
- **Asset Managers**: Image libraries, template collections, brand guidelines
- **Preview Tools**: Design mockups, print layouts, responsive previews
- **Collaboration Boards**: Design feedback, annotation tools, version control

#### 🔧 **Technical & Engineering**
- **Configuration Panels**: System settings, API endpoints, environment variables
- **Code Editors**: Syntax highlighting, error checking, auto-completion
- **Network Diagrams**: Infrastructure mapping, connection testing, monitoring
- **Data Flow Visualizers**: Pipeline builders, workflow designers, logic editors
- **Debugging Tools**: Log viewers, performance profilers, error trackers

#### 🎯 **Gaming & Entertainment**
- **Game Boards**: Chess, checkers, strategy games, puzzle interfaces
- **Leaderboards**: Scoring systems, achievement tracking, competition brackets
- **Virtual Environments**: 3D spaces, interactive scenarios, simulation controls
- **Character Builders**: RPG creation, avatar customization, skill trees
- **Tournament Brackets**: Competition organization, match tracking, results display

### Advanced Component Behaviors

#### **Multi-State Components**
Components that evolve through different states:
- **Wizard Flows**: Step-by-step processes with progress indicators
- **State Machines**: Complex workflows with conditional branching
- **Progressive Disclosure**: Revealing information based on user choices

#### **Real-Time Components**
Components with live data updates:
- **Live Dashboards**: Streaming metrics, real-time notifications
- **Collaborative Editing**: Multiple users interacting simultaneously
- **Dynamic Pricing**: Real-time rate updates, availability changes

#### **Contextual Components**
Components that adapt based on user or session context:
- **Personalized Interfaces**: User preference-driven layouts
- **Role-Based Views**: Different interfaces for different user types
- **Adaptive Complexity**: Simplified vs. advanced modes

#### **Integrated Components**
Components that work together:
- **Linked Visualizations**: Charts that update when maps are clicked
- **Component Chains**: Output from one feeds into another
- **Shared State**: Multiple components reflecting the same data

### Key Benefits
- **Dynamic UI**: Agents can spawn interactive components on-demand
- **Seamless Integration**: Components feel native to the chat experience
- **Extensible**: Easy to add new component types
- **Stateful**: Components can maintain state across interactions
- **Accessible**: Can be implemented with full accessibility support
- **Unlimited Creativity**: Any UI component imaginable can be implemented
- **Context-Aware**: Components can adapt based on conversation context
- **Real-Time Capable**: Support for live data updates and collaboration

### How It Works
1. **Agent Tool Call**: AI agent calls a special "display" tool
2. **Signal Generation**: Tool returns a special marker string instead of text
3. **API Processing**: Backend detects signal and adds it to message stream
4. **Frontend Detection**: UI watches for signals and renders components
5. **User Interaction**: Component interactions send normal chat messages

### Creative Implementation Ideas

#### **Industry-Specific Applications**

**Real Estate**: Property tours with 3D walkthroughs, mortgage calculators, neighborhood analytics, virtual staging tools

**Automotive**: Vehicle configurators, maintenance schedulers, diagnostic tools, trade-in estimators

**Fashion**: Virtual try-ons, style recommendations, size matching, trend visualizations

**Food Service**: Menu builders, dietary restriction filters, nutrition calculators, ordering interfaces

**Event Management**: Venue layouts, guest management, schedule builders, vendor coordination

**Legal Services**: Document assembly, case timelines, billing calculators, compliance checkers

**Architecture**: Blueprint viewers, material calculators, 3D renderings, cost estimators

**Manufacturing**: Production schedulers, quality control interfaces, supply chain visualizers

#### **Cross-Industry Patterns**

**Approval Workflows**: Multi-stage approval processes with role-based permissions

**Audit Trails**: Interactive timeline views of changes and decisions

**Resource Allocation**: Drag-and-drop scheduling and assignment tools

**Performance Monitoring**: Real-time dashboards with alert systems

**Communication Hubs**: Team collaboration spaces with integrated tools

The possibilities are truly limitless - any interactive user interface component you can imagine can be implemented using this pattern!

---

## Architecture Pattern

> **💡 Industry Standard**: This exact pattern is used by Slack Block Kit, Microsoft Teams Adaptive Cards, Discord interactive components, and GitHub's chat-based workflows. You're implementing a proven, enterprise-grade architecture pattern.

### Signal Flow Diagram
```
[AI Agent] → [Tool Call] → [Signal String] → [API Middleware] → [Message Stream] → [Frontend Router] → [UI Component]
     ↑                                                                                                    ↓
[Process Response] ← [Chat Message] ← [User Interaction] ← [Component Handler] ← [User Action]
```

### Core Components
1. **Signal Tools**: Backend functions that return marker strings (like Slack's Block Kit tools)
2. **Signal Parser**: API middleware that detects and processes signals (like Teams' adaptive card renderer)  
3. **Component Router**: Frontend logic that maps signals to components (like Discord's interaction handlers)
4. **Interactive Components**: UI elements that handle user interactions (like GitHub's review interfaces)

### Real-World Parallels
- **Slack**: `chat.postMessage` with `blocks` → Block Kit components appear in chat
- **Teams**: Adaptive card JSON → Interactive cards render in conversations  
- **Discord**: Slash command responses → Interactive components spawn
- **GitHub**: Bot comments with special formatting → Review/approval interfaces appear

---

## Backend Implementation

### 1. Define Signal Constants

```python
# signals.py
INTERACTIVE_SIGNALS = {
    # Basic Components
    "DISPLAY_SEAT_MAP": "seat_map",
    "DISPLAY_DATE_PICKER": "date_picker", 
    "DISPLAY_TIME_PICKER": "time_picker",
    
    # Data Visualizations
    "DISPLAY_CHART": "chart",
    "DISPLAY_MAP": "map",
    "DISPLAY_CALENDAR": "calendar",
    
    # Forms & Inputs
    "DISPLAY_FORM": "form",
    "DISPLAY_WIZARD": "wizard",
    "DISPLAY_SELECTOR": "selector",
    
    # Media & Rich Content
    "DISPLAY_IMAGE_GALLERY": "image_gallery",
    "DISPLAY_VIDEO_PLAYER": "video_player",
    "DISPLAY_DOCUMENT_VIEWER": "document_viewer",
    
    # Business-Specific
    "DISPLAY_PAYMENT_FORM": "payment_form",
    "DISPLAY_BOOKING_SUMMARY": "booking_summary",
    "DISPLAY_STATUS_TRACKER": "status_tracker"
}

class ComponentSignal:
    def __init__(self, signal_type: str, params: dict = None, metadata: dict = None):
        self.signal_type = signal_type
        self.params = params or {}
        self.metadata = metadata or {}
    
    def to_string(self) -> str:
        """Convert signal to string format"""
        if not self.params:
            return self.signal_type
        
        import json
        return f"{self.signal_type}:{json.dumps(self.params)}"
    
    @classmethod
    def from_string(cls, signal_string: str):
        """Parse signal from string format"""
        if ':' not in signal_string:
            return cls(signal_string)
        
        signal_type, params_json = signal_string.split(':', 1)
        try:
            import json
            params = json.loads(params_json)
            return cls(signal_type, params)
        except json.JSONDecodeError:
            return cls(signal_type, {"raw_params": params_json})
```

### 2. Create Signal Tools

```python
# tools.py
from typing import Any, Dict
import json

@function_tool(
    name_override="display_interactive_component",
    description_override="Display an interactive UI component to the user"
)
async def display_interactive_component(
    context: RunContextWrapper,
    component_type: str,
    **kwargs
) -> str:
    """
    Generic tool for displaying interactive components
    
    Args:
        component_type: Type of component to display
        **kwargs: Component-specific parameters
    """
    signal = ComponentSignal(f"DISPLAY_{component_type.upper()}", kwargs)
    return signal.to_string()

# Specific component tools
@function_tool
async def display_seat_map(
    context: RunContextWrapper,
    flight_number: str = None,
    aircraft_type: str = "narrow_body"
) -> str:
    """Display interactive seat selection map"""
    params = {
        "flight_number": flight_number,
        "aircraft_type": aircraft_type,
        "context_id": context.context.id if hasattr(context.context, 'id') else None
    }
    return ComponentSignal("DISPLAY_SEAT_MAP", params).to_string()

@function_tool 
async def display_date_picker(
    context: RunContextWrapper,
    purpose: str,
    min_date: str = None,
    max_date: str = None,
    selected_date: str = None
) -> str:
    """Display interactive date picker"""
    params = {
        "purpose": purpose,
        "min_date": min_date,
        "max_date": max_date, 
        "selected_date": selected_date
    }
    return ComponentSignal("DISPLAY_DATE_PICKER", params).to_string()

@function_tool
async def display_form(
    context: RunContextWrapper,
    form_type: str,
    fields: list,
    title: str = None
) -> str:
    """Display interactive form"""
    params = {
        "form_type": form_type,
        "fields": fields,
        "title": title
    }
    return ComponentSignal("DISPLAY_FORM", params).to_string()

@function_tool
async def display_chart(
    context: RunContextWrapper,
    chart_type: str,
    data: dict,
    title: str = None
) -> str:
    """Display interactive chart/visualization"""
    params = {
        "chart_type": chart_type,
        "data": data,
        "title": title
    }
    return ComponentSignal("DISPLAY_CHART", params).to_string()
```

### 3. Agent Configuration

```python
# agents.py
def create_interactive_agent():
    """Create agent with interactive UI capabilities"""
    
    interactive_tools = [
        display_seat_map,
        display_date_picker, 
        display_form,
        display_chart,
        display_interactive_component  # Generic fallback
    ]
    
    agent = Agent(
        name="Interactive Agent",
        model="gpt-4",
        instructions="""
        You are an agent capable of displaying interactive UI components.
        
        When users need to:
        - Select seats: Use display_seat_map
        - Pick dates: Use display_date_picker  
        - Fill forms: Use display_form
        - View data: Use display_chart
        
        Always explain what the component will help them accomplish.
        """,
        tools=interactive_tools
    )
    
    return agent
```

---

## API Middleware

### 1. Signal Detection & Processing

```python
# api_middleware.py
import re
from typing import List, Optional

class SignalProcessor:
    """Processes interactive component signals in API responses"""
    
    def __init__(self):
        self.signal_pattern = re.compile(r'^DISPLAY_[A-Z_]+(?:\:.*)?$')
    
    def is_signal(self, content: str) -> bool:
        """Check if content is a component signal"""
        return bool(self.signal_pattern.match(content.strip()))
    
    def parse_signal(self, content: str) -> ComponentSignal:
        """Parse signal from message content"""
        return ComponentSignal.from_string(content.strip())
    
    def process_tool_calls(self, tool_calls: List[ToolCallItem]) -> List[MessageResponse]:
        """Process tool calls and generate signal messages"""
        messages = []
        
        for tool_call in tool_calls:
            tool_name = getattr(tool_call.raw_item, "name", None)
            tool_output = tool_call.output if hasattr(tool_call, 'output') else None
            
            # Check if tool output is a signal
            if tool_output and self.is_signal(str(tool_output)):
                signal = self.parse_signal(str(tool_output))
                
                # Create signal message (hidden from chat display)
                messages.append(MessageResponse(
                    content=signal.to_string(),
                    agent=tool_call.agent.name,
                    message_type="signal",  # Mark as signal message
                    metadata={
                        "signal_type": signal.signal_type,
                        "params": signal.params,
                        "tool_name": tool_name
                    }
                ))
        
        return messages

# Enhanced API endpoint
@app.post("/chat")
async def chat_endpoint(req: ChatRequest):
    # ... existing conversation logic ...
    
    signal_processor = SignalProcessor()
    messages: List[MessageResponse] = []
    events: List[AgentEvent] = []
    
    for item in result.new_items:
        if isinstance(item, MessageOutputItem):
            # Regular text message
            text = ItemHelpers.text_message_output(item)
            messages.append(MessageResponse(
                content=text, 
                agent=item.agent.name,
                message_type="text"
            ))
            
        elif isinstance(item, ToolCallItem):
            # Process tool calls for signals
            signal_messages = signal_processor.process_tool_calls([item])
            messages.extend(signal_messages)
            
            # Log tool call event
            events.append(AgentEvent(
                id=uuid4().hex,
                type="tool_call",
                agent=item.agent.name,
                content=getattr(item.raw_item, "name", ""),
                metadata={"tool_args": getattr(item.raw_item, "arguments", {})}
            ))
    
    # ... rest of endpoint logic ...
```

### 2. Message Response Schema

```python
# schemas.py
from enum import Enum
from typing import Optional, Dict, Any

class MessageType(str, Enum):
    TEXT = "text"
    SIGNAL = "signal" 
    SYSTEM = "system"

class MessageResponse(BaseModel):
    content: str
    agent: str
    message_type: MessageType = MessageType.TEXT
    metadata: Optional[Dict[str, Any]] = None
    timestamp: Optional[float] = None
    
    class Config:
        use_enum_values = True

class ComponentSignalResponse(BaseModel):
    """Specific response for component signals"""
    signal_type: str
    params: Dict[str, Any] = {}
    component_id: Optional[str] = None
    requires_response: bool = True
```

---

## Frontend Implementation

### 1. Signal Detection Hook

```typescript
// hooks/useComponentSignals.ts
import { useEffect, useState } from 'react';
import { Message } from '@/lib/types';

export interface ComponentSignal {
  id: string;
  signalType: string;
  params: Record<string, any>;
  timestamp: number;
  agentName: string;
}

export function useComponentSignals(messages: Message[]) {
  const [activeSignals, setActiveSignals] = useState<ComponentSignal[]>([]);
  const [dismissedSignals, setDismissedSignals] = useState<Set<string>>(new Set());

  useEffect(() => {
    const signalMessages = messages.filter(
      msg => msg.role === 'assistant' && 
             msg.message_type === 'signal' &&
             msg.content.startsWith('DISPLAY_')
    );

    const signals: ComponentSignal[] = signalMessages
      .map((msg, index) => {
        const [signalType, paramsJson] = msg.content.split(':', 2);
        let params = {};
        
        if (paramsJson) {
          try {
            params = JSON.parse(paramsJson);
          } catch {
            params = { raw: paramsJson };
          }
        }

        return {
          id: `${msg.agent}-${signalType}-${index}`,
          signalType,
          params,
          timestamp: msg.timestamp || Date.now(),
          agentName: msg.agent
        };
      })
      .filter(signal => !dismissedSignals.has(signal.id));

    setActiveSignals(signals);
  }, [messages, dismissedSignals]);

  const dismissSignal = (id: string) => {
    setDismissedSignals(prev => new Set([...prev, id]));
  };

  const hasSignal = (signalType: string) => {
    return activeSignals.some(signal => signal.signalType === signalType);
  };

  return { activeSignals, dismissSignal, hasSignal };
}
```

### 2. Component Router

```typescript
// components/ComponentRouter.tsx
import React from 'react';
import { ComponentSignal } from '@/hooks/useComponentSignals';

// Import your interactive components
import { SeatMap } from './interactive/SeatMap';
import { DatePicker } from './interactive/DatePicker';
import { DynamicForm } from './interactive/DynamicForm';
import { InteractiveChart } from './interactive/InteractiveChart';

interface ComponentRouterProps {
  signals: ComponentSignal[];
  onComponentAction: (action: string, data: any, signalId: string) => void;
  onDismissSignal: (signalId: string) => void;
}

const COMPONENT_MAP = {
  'DISPLAY_SEAT_MAP': SeatMap,
  'DISPLAY_DATE_PICKER': DatePicker,
  'DISPLAY_FORM': DynamicForm,
  'DISPLAY_CHART': InteractiveChart,
  // Add more components as needed
} as const;

export function ComponentRouter({ 
  signals, 
  onComponentAction, 
  onDismissSignal 
}: ComponentRouterProps) {
  return (
    <div className="component-router">
      {signals.map((signal) => {
        const Component = COMPONENT_MAP[signal.signalType as keyof typeof COMPONENT_MAP];
        
        if (!Component) {
          console.warn(`No component found for signal: ${signal.signalType}`);
          return null;
        }

        return (
          <div 
            key={signal.id}
            className="interactive-component-wrapper"
            data-signal-type={signal.signalType}
            data-agent={signal.agentName}
          >
            <Component
              {...signal.params}
              signalId={signal.id}
              onAction={(action: string, data: any) => 
                onComponentAction(action, data, signal.id)
              }
              onDismiss={() => onDismissSignal(signal.id)}
            />
          </div>
        );
      })}
    </div>
  );
}
```

### 3. Enhanced Chat Component

```typescript
// components/Chat.tsx
import React, { useCallback } from 'react';
import { useComponentSignals } from '@/hooks/useComponentSignals';
import { ComponentRouter } from './ComponentRouter';

interface ChatProps {
  messages: Message[];
  onSendMessage: (message: string) => void;
  isLoading?: boolean;
}

export function Chat({ messages, onSendMessage, isLoading }: ChatProps) {
  const { activeSignals, dismissSignal, hasSignal } = useComponentSignals(messages);

  const handleComponentAction = useCallback((
    action: string, 
    data: any, 
    signalId: string
  ) => {
    // Convert component action to chat message
    let message = '';
    
    switch (action) {
      case 'seat_selected':
        message = `I would like seat ${data.seatNumber}`;
        break;
      case 'date_selected':
        message = `I choose ${data.date} for ${data.purpose}`;
        break;
      case 'form_submitted':
        message = `Form completed: ${JSON.stringify(data)}`;
        break;
      default:
        message = `${action}: ${JSON.stringify(data)}`;
    }
    
    // Dismiss the signal after action
    dismissSignal(signalId);
    
    // Send message to continue conversation
    onSendMessage(message);
  }, [dismissSignal, onSendMessage]);

  const filteredMessages = messages.filter(
    msg => msg.message_type !== 'signal'
  );

  return (
    <div className="chat-container">
      {/* Regular messages */}
      <div className="messages">
        {filteredMessages.map((msg, idx) => (
          <MessageBubble key={idx} message={msg} />
        ))}
        
        {/* Interactive components */}
        {activeSignals.length > 0 && (
          <div className="interactive-components">
            <ComponentRouter
              signals={activeSignals}
              onComponentAction={handleComponentAction}
              onDismissSignal={dismissSignal}
            />
          </div>
        )}
        
        {isLoading && <LoadingIndicator />}
      </div>
      
      {/* Input area */}
      <ChatInput onSendMessage={onSendMessage} />
    </div>
  );
}
```

---

## Component Examples

### 1. Interactive Seat Map

```typescript
// components/interactive/SeatMap.tsx
import React, { useState } from 'react';

interface SeatMapProps {
  flightNumber?: string;
  aircraftType?: string;
  signalId: string;
  onAction: (action: string, data: any) => void;
  onDismiss: () => void;
}

export function SeatMap({ 
  flightNumber, 
  aircraftType = 'narrow_body',
  signalId,
  onAction, 
  onDismiss 
}: SeatMapProps) {
  const [selectedSeat, setSelectedSeat] = useState<string | null>(null);

  const handleSeatClick = (seatNumber: string) => {
    setSelectedSeat(seatNumber);
  };

  const handleConfirm = () => {
    if (selectedSeat) {
      onAction('seat_selected', { 
        seatNumber: selectedSeat,
        flightNumber,
        aircraftType 
      });
    }
  };

  return (
    <div className="seat-map-container">
      <div className="seat-map-header">
        <h3>Select Your Seat</h3>
        {flightNumber && <p>Flight: {flightNumber}</p>}
        <button onClick={onDismiss} className="close-btn">×</button>
      </div>
      
      <div className="seat-grid">
        {/* Render seat layout based on aircraft type */}
        {/* Implementation details... */}
      </div>
      
      {selectedSeat && (
        <div className="seat-selection-footer">
          <p>Selected: {selectedSeat}</p>
          <button onClick={handleConfirm}>Confirm Selection</button>
        </div>
      )}
    </div>
  );
}
```

### 2. Dynamic Date Picker

```typescript
// components/interactive/DatePicker.tsx
import React, { useState } from 'react';

interface DatePickerProps {
  purpose: string;
  minDate?: string;
  maxDate?: string;
  selectedDate?: string;
  signalId: string;
  onAction: (action: string, data: any) => void;
  onDismiss: () => void;
}

export function DatePicker({
  purpose,
  minDate,
  maxDate,
  selectedDate,
  signalId,
  onAction,
  onDismiss
}: DatePickerProps) {
  const [currentDate, setCurrentDate] = useState(selectedDate || '');

  const handleDateSelect = (date: string) => {
    setCurrentDate(date);
    onAction('date_selected', { 
      date, 
      purpose,
      signalId 
    });
  };

  return (
    <div className="date-picker-container">
      <div className="date-picker-header">
        <h3>Select Date</h3>
        <p>{purpose}</p>
        <button onClick={onDismiss}>×</button>
      </div>
      
      <div className="calendar-widget">
        {/* Calendar implementation */}
        <input
          type="date"
          value={currentDate}
          min={minDate}
          max={maxDate}
          onChange={(e) => handleDateSelect(e.target.value)}
        />
      </div>
    </div>
  );
}
```

### 3. Dynamic Form Component

```typescript
// components/interactive/DynamicForm.tsx
import React, { useState } from 'react';

interface FormField {
  name: string;
  type: 'text' | 'email' | 'number' | 'select' | 'textarea';
  label: string;
  required?: boolean;
  options?: string[];
  placeholder?: string;
}

interface DynamicFormProps {
  formType: string;
  fields: FormField[];
  title?: string;
  signalId: string;
  onAction: (action: string, data: any) => void;
  onDismiss: () => void;
}

export function DynamicForm({
  formType,
  fields,
  title,
  signalId,
  onAction,
  onDismiss
}: DynamicFormProps) {
  const [formData, setFormData] = useState<Record<string, any>>({});
  const [errors, setErrors] = useState<Record<string, string>>({});

  const handleFieldChange = (fieldName: string, value: any) => {
    setFormData(prev => ({ ...prev, [fieldName]: value }));
    if (errors[fieldName]) {
      setErrors(prev => ({ ...prev, [fieldName]: '' }));
    }
  };

  const validateForm = () => {
    const newErrors: Record<string, string> = {};
    
    fields.forEach(field => {
      if (field.required && !formData[field.name]) {
        newErrors[field.name] = `${field.label} is required`;
      }
    });
    
    setErrors(newErrors);
    return Object.keys(newErrors).length === 0;
  };

  const handleSubmit = (e: React.FormEvent) => {
    e.preventDefault();
    
    if (validateForm()) {
      onAction('form_submitted', {
        formType,
        data: formData,
        signalId
      });
    }
  };

  return (
    <div className="dynamic-form-container">
      <div className="form-header">
        <h3>{title || `${formType} Form`}</h3>
        <button onClick={onDismiss}>×</button>
      </div>
      
      <form onSubmit={handleSubmit} className="dynamic-form">
        {fields.map(field => (
          <div key={field.name} className="form-field">
            <label htmlFor={field.name}>
              {field.label}
              {field.required && <span className="required">*</span>}
            </label>
            
            {field.type === 'select' ? (
              <select
                id={field.name}
                value={formData[field.name] || ''}
                onChange={(e) => handleFieldChange(field.name, e.target.value)}
              >
                <option value="">Select...</option>
                {field.options?.map(option => (
                  <option key={option} value={option}>{option}</option>
                ))}
              </select>
            ) : field.type === 'textarea' ? (
              <textarea
                id={field.name}
                value={formData[field.name] || ''}
                placeholder={field.placeholder}
                onChange={(e) => handleFieldChange(field.name, e.target.value)}
              />
            ) : (
              <input
                id={field.name}
                type={field.type}
                value={formData[field.name] || ''}
                placeholder={field.placeholder}
                onChange={(e) => handleFieldChange(field.name, e.target.value)}
              />
            )}
            
            {errors[field.name] && (
              <span className="error-message">{errors[field.name]}</span>
            )}
          </div>
        ))}
        
        <div className="form-actions">
          <button type="button" onClick={onDismiss}>Cancel</button>
          <button type="submit">Submit</button>
        </div>
      </form>
    </div>
  );
}
```

---

## Best Practices

### Reference: Learn from Production Systems
Before implementing your own patterns, study how established platforms handle interactive components:
- **[Slack Block Kit Examples](https://api.slack.com/block-kit)** - See JSON structures and interaction patterns
- **[Teams Adaptive Cards Samples](https://adaptivecards.io/samples/)** - Browse real-world card implementations  
- **[Discord Interactions Guide](https://discord.com/developers/docs/interactions/overview)** - Study slash command and button patterns

### 1. Signal Naming Convention (Industry Aligned)

```python
# Use consistent, descriptive signal names (like Slack's Block Kit naming)
SIGNAL_PATTERNS = {
    "Display Components": "DISPLAY_[COMPONENT_TYPE]",  # Like Slack's block types
    "Update State": "UPDATE_[STATE_TYPE]",             # Like Teams' card updates
    "Trigger Action": "TRIGGER_[ACTION_TYPE]",         # Like Discord's interactions
    "Request Input": "REQUEST_[INPUT_TYPE]"            # Like GitHub's input requests
}

# Examples:
# DISPLAY_SEAT_MAP
# DISPLAY_DATE_PICKER  
# UPDATE_USER_PREFERENCES
# TRIGGER_PAYMENT_FLOW
# REQUEST_CONFIRMATION
```

### 2. Parameter Validation

```python
# Validate signal parameters
from pydantic import BaseModel, validator

class SeatMapParams(BaseModel):
    flight_number: Optional[str] = None
    aircraft_type: str = "narrow_body"
    preferred_section: Optional[str] = None
    
    @validator('aircraft_type')
    def validate_aircraft_type(cls, v):
        allowed_types = ['narrow_body', 'wide_body', 'regional']
        if v not in allowed_types:
            raise ValueError(f'aircraft_type must be one of {allowed_types}')
        return v

@function_tool
async def display_seat_map_validated(
    context: RunContextWrapper,
    **kwargs
) -> str:
    """Display seat map with parameter validation"""
    try:
        params = SeatMapParams(**kwargs)
        return ComponentSignal("DISPLAY_SEAT_MAP", params.dict()).to_string()
    except ValueError as e:
        return f"Error: {str(e)}"
```

### 3. Error Handling

```typescript
// Handle component errors gracefully
export function ComponentRouter({ signals, onComponentAction, onDismissSignal }: ComponentRouterProps) {
  const [componentErrors, setComponentErrors] = useState<Record<string, string>>({});

  const handleComponentError = (signalId: string, error: Error) => {
    console.error(`Component error for ${signalId}:`, error);
    setComponentErrors(prev => ({
      ...prev,
      [signalId]: error.message
    }));
  };

  return (
    <div className="component-router">
      {signals.map((signal) => {
        if (componentErrors[signal.id]) {
          return (
            <div key={signal.id} className="component-error">
              <p>Failed to load component: {componentErrors[signal.id]}</p>
              <button onClick={() => onDismissSignal(signal.id)}>Dismiss</button>
            </div>
          );
        }

        // ... render component with error boundary
      })}
    </div>
  );
}
```

### 4. State Persistence

```typescript
// Persist component state across page reloads
export function usePersistedComponentState(signalId: string) {
  const [state, setState] = useState(() => {
    const stored = localStorage.getItem(`component_state_${signalId}`);
    return stored ? JSON.parse(stored) : {};
  });

  useEffect(() => {
    localStorage.setItem(`component_state_${signalId}`, JSON.stringify(state));
  }, [signalId, state]);

  return [state, setState];
}
```

### 5. Accessibility

```typescript
// Ensure components are accessible
export function AccessibleComponent({ children, signalType, ...props }) {
  return (
    <div
      role="dialog"
      aria-labelledby={`${signalType}-title`}
      aria-describedby={`${signalType}-description`}
      {...props}
    >
      {children}
    </div>
  );
}
```

---

## Advanced Patterns

### 1. Component Chaining

```python
@function_tool
async def display_component_chain(
    context: RunContextWrapper,
    components: List[str],
    data: dict = None
) -> str:
    """Display multiple components in sequence"""
    chain_data = {
        "components": components,
        "current_index": 0,
        "data": data or {}
    }
    return ComponentSignal("DISPLAY_CHAIN", chain_data).to_string()
```

### 2. Conditional Components

```python
@function_tool
async def display_conditional_component(
    context: RunContextWrapper,
    condition_key: str,
    condition_value: Any,
    true_component: str,
    false_component: str,
    **params
) -> str:
    """Display component based on condition"""
    context_value = getattr(context.context, condition_key, None)
    
    if context_value == condition_value:
        component_type = true_component
    else:
        component_type = false_component
    
    return ComponentSignal(f"DISPLAY_{component_type.upper()}", params).to_string()
```

### 3. Real-time Components

```typescript
// Real-time data streaming to components
export function useRealTimeData(endpoint: string, signalId: string) {
  const [data, setData] = useState(null);
  const [isConnected, setIsConnected] = useState(false);

  useEffect(() => {
    const ws = new WebSocket(endpoint);
    
    ws.onopen = () => setIsConnected(true);
    ws.onmessage = (event) => {
      const newData = JSON.parse(event.data);
      setData(newData);
    };
    ws.onclose = () => setIsConnected(false);

    return () => ws.close();
  }, [endpoint]);

  return { data, isConnected };
}
```

---

## Testing & Debugging

### 1. Signal Testing

```python
# test_signals.py
import pytest
from your_app.signals import ComponentSignal

def test_signal_creation():
    signal = ComponentSignal("DISPLAY_SEAT_MAP", {"flight": "AA123"})
    assert signal.to_string() == 'DISPLAY_SEAT_MAP:{"flight": "AA123"}'

def test_signal_parsing():
    signal_string = 'DISPLAY_DATE_PICKER:{"purpose": "departure"}'
    signal = ComponentSignal.from_string(signal_string)
    assert signal.signal_type == "DISPLAY_DATE_PICKER"
    assert signal.params["purpose"] == "departure"

@pytest.mark.asyncio
async def test_display_tool():
    context = create_test_context()
    result = await display_seat_map(context, flight_number="AA123")
    assert "DISPLAY_SEAT_MAP" in result
```

### 2. Component Testing

```typescript
// SeatMap.test.tsx
import { render, fireEvent, screen } from '@testing-library/react';
import { SeatMap } from './SeatMap';

describe('SeatMap Component', () => {
  const mockOnAction = jest.fn();
  const mockOnDismiss = jest.fn();

  beforeEach(() => {
    jest.clearAllMocks();
  });

  test('renders seat map with flight number', () => {
    render(
      <SeatMap
        flightNumber="AA123"
        signalId="test-signal"
        onAction={mockOnAction}
        onDismiss={mockOnDismiss}
      />
    );

    expect(screen.getByText('Flight: AA123')).toBeInTheDocument();
  });

  test('calls onAction when seat is selected', () => {
    render(
      <SeatMap
        flightNumber="AA123"
        signalId="test-signal"
        onAction={mockOnAction}
        onDismiss={mockOnDismiss}
      />
    );

    // Simulate seat selection
    const seat = screen.getByTestId('seat-1A');
    fireEvent.click(seat);
    
    const confirmButton = screen.getByText('Confirm Selection');
    fireEvent.click(confirmButton);

    expect(mockOnAction).toHaveBeenCalledWith('seat_selected', {
      seatNumber: '1A',
      flightNumber: 'AA123',
      aircraftType: 'narrow_body'
    });
  });
});
```

### 3. Debug Tools

```typescript
// Development debug panel
export function SignalDebugPanel({ signals }: { signals: ComponentSignal[] }) {
  if (process.env.NODE_ENV !== 'development') return null;

  return (
    <div className="signal-debug-panel">
      <h4>Active Signals</h4>
      {signals.map(signal => (
        <div key={signal.id} className="debug-signal">
          <strong>{signal.signalType}</strong>
          <pre>{JSON.stringify(signal.params, null, 2)}</pre>
        </div>
      ))}
    </div>
  );
}
```

---

## Security Considerations

> **🔒 Learn from Enterprise**: Study how [Slack](https://api.slack.com/security), [Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/deploy-and-publish/appsource/prepare/security-review), and [Discord](https://discord.com/developers/docs/legal) handle security in their interactive components. They provide excellent examples of input validation, XSS prevention, and secure state management.

### 1. Input Sanitization (Platform Standards)

```python
# Sanitize signal parameters
import html
from typing import Any, Dict

def sanitize_signal_params(params: Dict[str, Any]) -> Dict[str, Any]:
    """Sanitize parameters to prevent XSS"""
    sanitized = {}
    
    for key, value in params.items():
        if isinstance(value, str):
            sanitized[key] = html.escape(value)
        elif isinstance(value, dict):
            sanitized[key] = sanitize_signal_params(value)
        elif isinstance(value, list):
            sanitized[key] = [html.escape(v) if isinstance(v, str) else v for v in value]
        else:
            sanitized[key] = value
    
    return sanitized
```

### 2. Signal Validation

```python
# Validate signals against allowed types
ALLOWED_SIGNALS = {
    "DISPLAY_SEAT_MAP",
    "DISPLAY_DATE_PICKER", 
    "DISPLAY_FORM",
    "DISPLAY_CHART"
}

def validate_signal(signal_type: str) -> bool:
    """Validate signal type against allowlist"""
    return signal_type in ALLOWED_SIGNALS

@function_tool
async def secure_display_component(
    context: RunContextWrapper,
    component_type: str,
    **kwargs
) -> str:
    """Securely display component with validation"""
    signal_type = f"DISPLAY_{component_type.upper()}"
    
    if not validate_signal(signal_type):
        raise ValueError(f"Signal type {signal_type} not allowed")
    
    sanitized_params = sanitize_signal_params(kwargs)
    return ComponentSignal(signal_type, sanitized_params).to_string()
```

### 3. Rate Limiting

```typescript
// Rate limit component signals
export function useSignalRateLimit(maxSignalsPerMinute = 10) {
  const [signalTimestamps, setSignalTimestamps] = useState<number[]>([]);

  const canProcessSignal = useCallback(() => {
    const now = Date.now();
    const oneMinuteAgo = now - 60000;
    const recentSignals = signalTimestamps.filter(ts => ts > oneMinuteAgo);
    
    return recentSignals.length < maxSignalsPerMinute;
  }, [signalTimestamps, maxSignalsPerMinute]);

  const recordSignal = useCallback(() => {
    setSignalTimestamps(prev => [...prev, Date.now()]);
  }, []);

  return { canProcessSignal, recordSignal };
}
```

---

## Conclusion

This signal-based pattern provides a powerful way to create rich, interactive experiences within conversational AI applications. **You're implementing the same architecture pattern used by industry leaders like Slack, Microsoft Teams, Discord, and GitHub** - a proven, enterprise-grade approach to chat-based interactive components.

### Key Benefits Include:
- **Industry-Standard Architecture**: Following patterns used by millions of users daily
- **Flexibility**: Easy to add new component types (like Slack's expanding Block Kit library)
- **Separation of Concerns**: Clean separation between AI logic and UI (like Teams' adaptive cards)
- **User Experience**: Seamless integration of complex interactions (like Discord's slash commands)
- **Maintainability**: Modular, testable architecture (like GitHub's review workflows)

### Next Steps:
1. **Study the live examples** linked at the top of this guide
2. **Explore existing implementations** in Slack, Teams, and Discord
3. **Start with simple components** and gradually add complexity
4. **Follow security best practices** from established platforms
5. **Test extensively** with real users to refine the experience

By following this implementation guide and learning from production systems, you can create sophisticated agent-based applications that feel more like native applications while maintaining the conversational flow that users expect from AI assistants.

### Resources for Continued Learning:
- **[Slack Developer Documentation](https://api.slack.com/)** - Comprehensive guides and examples
- **[Microsoft Teams Platform](https://docs.microsoft.com/en-us/microsoftteams/platform/)** - Adaptive cards and bot frameworks
- **[Discord Developer Portal](https://discord.com/developers/docs)** - Interaction patterns and components
- **[GitHub Apps Documentation](https://docs.github.com/en/developers/apps)** - Chat-based workflow examples

Remember: You're not just building a custom solution - you're implementing a pattern that powers some of the world's most successful collaboration platforms. 🚀 