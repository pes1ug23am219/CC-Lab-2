# **Lab 2: Monolithic App Optimization**

## **What We Did**
1. **Set up a monolithic FastAPI app** simulating a college fest system (registration, events, checkout, dashboard)
2. **Demonstrated monolithic failure** - intentionally crashed the checkout page, bringing down the entire app
3. **Fixed the bug** and restored functionality
4. **Load tested** using Locust to measure performance
5. **Optimized three endpoints** by removing inefficient loops and redundant computations:
   - `/checkout` - Reduced response time from ~113ms to ~107ms
   - `/events` - Eliminated CPU-intensive loop, improved throughput
   - `/myevents` - Removed unnecessary loop, better concurrency

## **Key Takeaway**
Monolithic apps are simple to build but have a **single point of failure** - one bug can crash everything. We improved performance by removing inefficient code, but scaling remains challenging with this architecture.

**SRN:** PES1UG23AM219
