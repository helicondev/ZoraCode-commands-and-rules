# Database Performance Analyzer Command

A command to systematically analyze the database performance.

## Usage
/database-performance-analyzer [file-path]

## Template
Use the following systematic approach to analyze the database performance:

{{input}}

SYSTEMATIC PERFORMANCE ANALYSIS:
1. QUERY OPTIMIZATION AUDIT:
   - Identify missing indexes using query execution plans
   - Check for table scans on large tables (>1M rows)
   - Analyze JOIN complexity and optimization opportunities
   - Verify WHERE clause selectivity and index usage

2. SCHEMA DESIGN EVALUATION:
   - Check normalization level appropriateness
   - Identify denormalization opportunities for read-heavy workloads
   - Analyze data type efficiency (INT vs BIGINT, VARCHAR sizing)
   - Verify foreign key constraints and their performance impact

3. CONCURRENCY & LOCKING ANALYSIS:
   - Identify potential deadlock scenarios
   - Check transaction isolation level appropriateness
   - Analyze long-running transaction impact
   - Verify connection pooling configuration

4. SCALING BOTTLENECK IDENTIFICATION:
   - Project performance at 10x, 100x current data volume
   - Identify single points of failure in architecture
   - Analyze read/write ratio and sharding opportunities
   - Check replication lag and consistency requirements

5. MAINTENANCE & MONITORING:
   - Verify backup strategy performance impact
   - Check statistics update frequency and accuracy
   - Analyze slow query log patterns
   - Review disk space growth projections

DELIVERABLE: Performance optimization roadmap with specific query rewrites, index recommendations, and scaling strategy with timeline.