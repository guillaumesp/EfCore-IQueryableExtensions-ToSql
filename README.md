# EfCore-IQueryableExtensions-ToSql
EfCore 2.1 Preview IQueryableExtensions

## Accessing SQL from Entity Framework Core Queries

Based on Ricardo Peres work

Usage
```
// Build a query using Entity Framework
var query = _context.Widgets.Where(w => w.IsReal && w.Id == 42);  
// Get the generated SQL
var sql = query.ToSql();
```