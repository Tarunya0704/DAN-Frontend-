
![Screenshot 2024-12-22 122040](https://github.com/user-attachments/assets/6f3af865-1746-4a95-8193-c9d2680cc375)
# Decentralized Autonomous Network (DAN)

A Next.js-based dashboard for monitoring and managing decentralized network nodes with real-time metrics visualization.

## Features

- 🌓 Dark/Light mode support with system preference detection
- 📊 Real-time performance monitoring with interactive charts
- 🌍 Multi-region node deployment simulation
- 📈 Node metrics tracking (CPU, Memory, Network)
- 🔄 Automatic metrics updates every 5 seconds
- 🎨 Responsive design with Tailwind CSS
- 📱 Mobile-friendly interface

## Prerequisites

Before you begin, ensure you have installed:
- Node.js (v14.0.0 or higher)
- npm (v6.0.0 or higher)

## Installation

1. Clone the repository:
```bash
git clone <your-repository-url>
cd dan
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Install required dependencies:
```bash
npm install recharts lucide-react
```

## Running the Application

1. Start the development server:
```bash
npm run dev
# or
yarn dev
```

2. Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

```
src/
├── app/
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── components/
│   └── NodeGenerator.tsx    # Main component
└── styles/
    └── tailwind.css
```

## Features Breakdown

### Node Generation
- Customizable node count
- Region-specific IP address allocation
- Unique node naming with custom prefixes
- Simulated node creation with loading states

### Performance Monitoring
- Real-time CPU usage tracking
- Memory utilization monitoring
- Network bandwidth visualization
- Status indicators for each node

### Dark Mode
- System preference detection
- Manual toggle option
- Persistent preference storage

### Metrics Dashboard
- Line charts for CPU and memory trends
- Real-time metric updates
- Comprehensive node status table
- Network performance monitoring

## Available Regions

- US-East
- US-West
- EU-West
- EU-Central
- Asia-Pacific

## Technical Details

### IP Address Allocation

Each region has a dedicated IP range:
- US-East: 10.0.0.0 - 10.0.255.255
- US-West: 10.1.0.0 - 10.1.255.255
- EU-West: 10.2.0.0 - 10.2.255.255
- EU-Central: 10.3.0.0 - 10.3.255.255
- Asia-Pacific: 10.4.0.0 - 10.4.255.255

### Metrics Update Cycle

- Metrics are updated every 5 seconds
- Each update includes:
  - CPU utilization
  - Memory usage
  - Network bandwidth
  - Node status (online/offline)
  - Historical performance data

## Customization

### Styling

The project uses Tailwind CSS for styling. You can customize the appearance by:

1. Modifying the Tailwind configuration in `tailwind.config.js`
2. Adding custom CSS in `globals.css`
3. Updating component-specific styles in the JSX

### Metrics Simulation

You can adjust the metrics simulation by modifying:
- Update frequency in the `useEffect` hook
- Range of generated values for CPU, memory, and network metrics
- Historical data retention period

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/new-feature`
3. Commit changes: `git commit -am 'Add new feature'`
4. Push to the branch: `git push origin feature/new-feature`
5. Submit a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

