[Option<T>](https://doc.rust-lang.org/std/option/enum.Option.html)
## To inner type
fn  [unwrap](https://doc.rust-lang.org/std/option/enum.Option.html#method.unwrap) () -> T
fn  [unwrap_or](https://doc.rust-lang.org/std/option/enum.Option.html#method.unwrap_or) (T) -> T
fn  [unwrap_or_else](https://doc.rust-lang.org/std/option/enum.Option.html#method.unwrap_or_else) (() -> T) -> T
fn  [unwrap_or_default](https://doc.rust-lang.org/std/option/enum.Option.html#method.unwrap_or_default) () -> T where  T: [Default](https://doc.rust-lang.org/std/default/trait.Default.html)
fn  [expect](https://doc.rust-lang.org/std/option/enum.Option.html#method.expect) (& [str](https://doc.rust-lang.org/std/primitive.str.html)) -> T
## Converting to another type
fn  [map](https://doc.rust-lang.org/std/option/enum.Option.html#method.map) ((T) -> U) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<U>
fn  [map_or](https://doc.rust-lang.org/std/option/enum.Option.html#method.map_or) (U, (T) -> U) -> U
fn  [map_or_else](https://doc.rust-lang.org/std/option/enum.Option.html#method.map_or_else) (() -> U, (T) -> U) -> U
## To Result
fn  [ok_or](https://doc.rust-lang.org/std/option/enum.Option.html#method.ok_or) (E) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<T, E>
fn  [ok_or_else](https://doc.rust-lang.org/std/option/enum.Option.html#method.ok_or_else) (() -> E) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<T, E>
## Conditioning
fn  [filter](https://doc.rust-lang.org/std/option/enum.Option.html#method.filter) ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [and](https://doc.rust-lang.org/std/option/enum.Option.html#method.and) ([Option](https://doc.rust-lang.org/std/option/enum.Option.html)<U>) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<U>
fn  [and_then](https://doc.rust-lang.org/std/option/enum.Option.html#method.and_then) ((T) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<U>) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<U>
fn  [or](https://doc.rust-lang.org/std/option/enum.Option.html#method.or) ([Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [or_else](https://doc.rust-lang.org/std/option/enum.Option.html#method.or_else) (() -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
[Option<&T>](https://doc.rust-lang.org/std/option/enum.Option.html)
## Cloning inner
fn  [cloned](https://doc.rust-lang.org/std/option/enum.Option.html#method.cloned) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T> where  T: [Clone](https://doc.rust-lang.org/std/clone/trait.Clone.html)
[Option<Result<T, E>>](https://doc.rust-lang.org/std/option/enum.Option.html)
## Transposing
fn  [transpose](https://doc.rust-lang.org/std/option/enum.Option.html#method.transpose) () -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<[Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>, E>
[&Option<T>](https://doc.rust-lang.org/std/option/enum.Option.html)
## Checking inner
fn  [is_some](https://doc.rust-lang.org/std/option/enum.Option.html#method.is_some) () -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
fn  [is_none](https://doc.rust-lang.org/std/option/enum.Option.html#method.is_none) () -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
## To inner reference
fn  [as_ref](https://doc.rust-lang.org/std/option/enum.Option.html#method.as_ref) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<& T>
fn  [iter](https://doc.rust-lang.org/std/option/enum.Option.html#method.iter) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<& T>
[&mut Option<T>](https://doc.rust-lang.org/std/option/enum.Option.html)
## To inner mutable reference
fn  [as_mut](https://doc.rust-lang.org/std/option/enum.Option.html#method.as_mut) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<& mut  T>
fn  [iter_mut](https://doc.rust-lang.org/std/option/enum.Option.html#method.iter_mut) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<& mut  T>
## Mutation
fn  [take](https://doc.rust-lang.org/std/option/enum.Option.html#method.take) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [replace](https://doc.rust-lang.org/std/option/enum.Option.html#method.replace) (T) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [get_or_insert](https://doc.rust-lang.org/std/option/enum.Option.html#method.get_or_insert) (T) -> & mut  T
fn  [get_or_insert_with](https://doc.rust-lang.org/std/option/enum.Option.html#method.get_or_insert_with) (() -> T) -> & mut  T
[Result<T, E>](https://doc.rust-lang.org/std/result/enum.Result.html)
## To inner type
fn  [unwrap](https://doc.rust-lang.org/std/result/enum.Result.html#method.unwrap) () -> T where  E: [Debug](https://doc.rust-lang.org/std/fmt/trait.Debug.html)
fn  [unwrap_err](https://doc.rust-lang.org/std/result/enum.Result.html#method.unwrap_err) () -> E where  T: [Debug](https://doc.rust-lang.org/std/fmt/trait.Debug.html)
fn  [unwrap_or](https://doc.rust-lang.org/std/result/enum.Result.html#method.unwrap_or) (T) -> T
fn  [unwrap_or_else](https://doc.rust-lang.org/std/result/enum.Result.html#method.unwrap_or_else) ((E) -> T) -> T
fn  [unwrap_or_default](https://doc.rust-lang.org/std/result/enum.Result.html#method.unwrap_or_default) () -> T where  T: [Default](https://doc.rust-lang.org/std/default/trait.Default.html)
fn  [expect](https://doc.rust-lang.org/std/result/enum.Result.html#method.expect) (& [str](https://doc.rust-lang.org/std/primitive.str.html)) -> T
fn  [expect_err](https://doc.rust-lang.org/std/result/enum.Result.html#method.expect_err) (& [str](https://doc.rust-lang.org/std/primitive.str.html)) -> E
fn  [ok](https://doc.rust-lang.org/std/result/enum.Result.html#method.ok) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [err](https://doc.rust-lang.org/std/result/enum.Result.html#method.err) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<E>
## Mapping
fn  [map](https://doc.rust-lang.org/std/result/enum.Result.html#method.map) ((T) -> U) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<U, E>
fn  [map_err](https://doc.rust-lang.org/std/result/enum.Result.html#method.map_err) ((E) -> F) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<T, F>
## Conditioning
fn  [and](https://doc.rust-lang.org/std/result/enum.Result.html#method.and) ([Result](https://doc.rust-lang.org/std/result/enum.Result.html)<U, E>) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<U, E>
fn  [and_then](https://doc.rust-lang.org/std/result/enum.Result.html#method.and_then) ((T) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<U, E>) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<U, E>
fn  [or](https://doc.rust-lang.org/std/result/enum.Result.html#method.or) ([Result](https://doc.rust-lang.org/std/result/enum.Result.html)<T, F>) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<T, F>
fn  [or_else](https://doc.rust-lang.org/std/result/enum.Result.html#method.or_else) ((E) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<T, F>) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<T, F>
[Result<Option<T>, E>](https://doc.rust-lang.org/std/result/enum.Result.html)
## Transposing
fn  [transpose](https://doc.rust-lang.org/std/result/enum.Result.html#method.transpose) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<[Result](https://doc.rust-lang.org/std/result/enum.Result.html)<T, E>>
[&Result<T, E>](https://doc.rust-lang.org/std/result/enum.Result.html)
## Checking inner
fn  [is_ok](https://doc.rust-lang.org/std/result/enum.Result.html#method.is_ok) () -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
fn  [is_err](https://doc.rust-lang.org/std/result/enum.Result.html#method.is_err) () -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
## To inner reference
fn  [as_ref](https://doc.rust-lang.org/std/result/enum.Result.html#method.as_ref) () -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<& T, & E>
fn  [iter](https://doc.rust-lang.org/std/result/enum.Result.html#method.iter) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & T>
[&mut Result<T, E>](https://doc.rust-lang.org/std/result/enum.Result.html)
## To inner mutable reference
fn  [as_mut](https://doc.rust-lang.org/std/result/enum.Result.html#method.as_mut) () -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<& mut  T, & mut  E>
fn  [iter_mut](https://doc.rust-lang.org/std/result/enum.Result.html#method.iter_mut) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  T>
[Iterator<Item = T>](https://doc.rust-lang.org/std/iter/trait.Iterator.html)
## Mapping and filtering
fn  [map](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.map)        (( T) -> U)         -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = U>
fn  [filter](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.filter)     ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html))      -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [filter_map](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.filter_map) (( T) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<U>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = U>
## Collecting and folding
fn  [fold](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.fold) (S, (S, T) -> S) -> S
fn  [collect](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.collect) () -> B where  B: [FromIterator](https://doc.rust-lang.org/std/iter/trait.FromIterator.html)<T>
fn  [partition](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.partition) ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> (B, B) where  B: [Default](https://doc.rust-lang.org/std/default/trait.Default.html) + [Extend](https://doc.rust-lang.org/std/iter/trait.Extend.html)<T>
## Counting and enumerating
fn  [count](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.count) () -> [usize](https://doc.rust-lang.org/std/primitive.usize.html)
fn  [last](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.last) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [enumerate](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.enumerate) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = ([usize](https://doc.rust-lang.org/std/primitive.usize.html), T)>
## Combining with other iterators
fn  [zip](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.zip)   ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = U>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = (T, U)>
fn  [chain](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.chain) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
## Flattening
fn  [flatten](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.flatten) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<U> where  T: [IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<U>
fn  [flat_map](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.flat_map) ((T) -> [IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = U>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = U>
## Taking and skipping
fn  [skip](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.skip) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [take](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.take) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [skip_while](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.skip_while) ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [take_while](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.take_while) ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [step_by](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.step_by) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
## Misc. iterating
fn  [for_each](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.for_each) ((T) -> ()) -> ()
fn  [inspect](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.inspect) ((& T) -> ()) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [scan](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.scan) (S, (& mut  S, T) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<U>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = U>
## Calculations
fn  [sum](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.sum)     () -> S where  S: [Sum](https://doc.rust-lang.org/std/iter/trait.Sum.html)<T>
fn  [product](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.product) () -> P where  P: [Product](https://doc.rust-lang.org/std/iter/trait.Product.html)<T>
## Maximum and minimum
fn  [max](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.max) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T> where  T: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
fn  [min](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.min) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T> where  T: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
fn  [max_by](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.max_by) ((& T, & T) -> [Ordering](https://doc.rust-lang.org/std/cmp/enum.Ordering.html)) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [min_by](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.min_by) ((& T, & T) -> [Ordering](https://doc.rust-lang.org/std/cmp/enum.Ordering.html)) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [max_by_key](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.max_by_key) ((& T) -> U) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T> where  U: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
fn  [min_by_key](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.min_by_key) ((& T) -> U) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T> where  U: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
## Comparing with another iterator
fn  [eq](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.eq) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html) where  T: [PartialEq](https://doc.rust-lang.org/std/cmp/trait.PartialEq.html)
fn  [ne](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.ne) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html) where  T: [PartialEq](https://doc.rust-lang.org/std/cmp/trait.PartialEq.html)
fn  [lt](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.lt) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html) where  T: [PartialOrd](https://doc.rust-lang.org/std/cmp/trait.PartialOrd.html)
fn  [le](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.le) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html) where  T: [PartialOrd](https://doc.rust-lang.org/std/cmp/trait.PartialOrd.html)
fn  [gt](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.gt) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html) where  T: [PartialOrd](https://doc.rust-lang.org/std/cmp/trait.PartialOrd.html)
fn  [ge](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.ge) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html) where  T: [PartialOrd](https://doc.rust-lang.org/std/cmp/trait.PartialOrd.html)
fn  [cmp](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.cmp) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>) -> [Ordering](https://doc.rust-lang.org/std/cmp/enum.Ordering.html) where  T: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
fn  [partial_cmp](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.partial_cmp) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>)-> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<[Ordering](https://doc.rust-lang.org/std/cmp/enum.Ordering.html)> where  T: [PartialOrd](https://doc.rust-lang.org/std/cmp/trait.PartialOrd.html)
## Reversing and cycling
fn  [rev](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.rev)   () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T> where  Self: [DoubleEndedIterator](https://doc.rust-lang.org/std/iter/trait.DoubleEndedIterator.html)
fn  [cycle](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.cycle) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T> where  Self: [Clone](https://doc.rust-lang.org/std/clone/trait.Clone.html)
[Iterator<Item = &T>](https://doc.rust-lang.org/std/iter/trait.Iterator.html)
## Cloning inner
fn  [cloned](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.cloned) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<T> where  T: [Clone](https://doc.rust-lang.org/std/clone/trait.Clone.html)
[&mut Iterator<Item = T>](https://doc.rust-lang.org/std/iter/trait.Iterator.html)
## Finding and positioning
fn  [find](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.find)      ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html))      -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [find_map](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.find_map)  (( T) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<U>) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<U>
fn  [position](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.position)  (( T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html))      -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>
fn  [rposition](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.rposition) (( T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html))      -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>where  Self: [ExactSizeIterator](https://doc.rust-lang.org/std/iter/trait.ExactSizeIterator.html) + [DoubleEndedIterator](https://doc.rust-lang.org/std/iter/trait.DoubleEndedIterator.html)
## Boolean operations
fn  [all](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.all) ((T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
fn  [any](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.any) ((T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
## Try iterating
fn  [try_for_each](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.try_for_each) ((T) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<()>)    -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<()>
fn  [try_for_each](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.try_for_each) ((T) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<(), E>) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<(), E>
fn  [try_fold](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.try_fold) (S, (S, T) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<S>)    -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<S>
fn  [try_fold](https://doc.rust-lang.org/std/iter/trait.Iterator.html#method.try_fold) (S, (S, T) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<S, E>) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<S, E>
[std::iter](https://doc.rust-lang.org/std/iter/)
## Creating simple iterators
fn  [empty](https://doc.rust-lang.org/std/iter/fn.empty.html) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [once](https://doc.rust-lang.org/std/iter/fn.once.html) (T) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [repeat](https://doc.rust-lang.org/std/iter/fn.repeat.html) (T) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T> where  T: [Clone](https://doc.rust-lang.org/std/clone/trait.Clone.html)
fn  [repeat_with](https://doc.rust-lang.org/std/iter/fn.repeat_with.html) (() -> T) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [from_fn](https://doc.rust-lang.org/std/iter/fn.from_fn.html) (() -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
fn  [successors](https://doc.rust-lang.org/std/iter/fn.successors.html) ([Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>, (& T) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = T>
[&[T]](https://doc.rust-lang.org/std/primitive.slice.html)
## Splitting to iterator
fn  [split](https://doc.rust-lang.org/std/primitive.slice.html#method.split)  ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [T]>
fn  [rsplit](https://doc.rust-lang.org/std/primitive.slice.html#method.rsplit) ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [T]>
fn  [splitn](https://doc.rust-lang.org/std/primitive.slice.html#method.splitn)  ([usize](https://doc.rust-lang.org/std/primitive.usize.html), (& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [T]>
fn  [rsplitn](https://doc.rust-lang.org/std/primitive.slice.html#method.rsplitn) ([usize](https://doc.rust-lang.org/std/primitive.usize.html), (& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [T]>
## Splitting at position
fn  [split_at](https://doc.rust-lang.org/std/primitive.slice.html#method.split_at) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> (& [T], & [T])
fn  [split_first](https://doc.rust-lang.org/std/primitive.slice.html#method.split_first) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<(& T, & [T])>
fn  [split_last](https://doc.rust-lang.org/std/primitive.slice.html#method.split_last)  () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<(& T, & [T])>
## Chunks and windows
fn  [chunks](https://doc.rust-lang.org/std/primitive.slice.html#method.chunks)        ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [T]>
fn  [chunks_exact](https://doc.rust-lang.org/std/primitive.slice.html#method.chunks_exact)  ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [T]>
fn  [rchunks](https://doc.rust-lang.org/std/primitive.slice.html#method.rchunks)       ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [T]>
fn  [rchunks_exact](https://doc.rust-lang.org/std/primitive.slice.html#method.rchunks_exact) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [T]>
fn  [windows](https://doc.rust-lang.org/std/primitive.slice.html#method.windows)       ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [T]>
## Matching
fn  [contains](https://doc.rust-lang.org/std/primitive.slice.html#method.contains)    (& T)   -> [bool](https://doc.rust-lang.org/std/primitive.bool.html) where  T: [PartialEq](https://doc.rust-lang.org/std/cmp/trait.PartialEq.html)
fn  [starts_with](https://doc.rust-lang.org/std/primitive.slice.html#method.starts_with) (& [T]) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html) where  T: [PartialEq](https://doc.rust-lang.org/std/cmp/trait.PartialEq.html)
fn  [ends_with](https://doc.rust-lang.org/std/primitive.slice.html#method.ends_with)   (& [T]) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html) where  T: [PartialEq](https://doc.rust-lang.org/std/cmp/trait.PartialEq.html)
## Binary searching
fn  [binary_search](https://doc.rust-lang.org/std/primitive.slice.html#method.binary_search) (& T)                   -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html), [usize](https://doc.rust-lang.org/std/primitive.usize.html)> where  T: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
fn  [binary_search_by](https://doc.rust-lang.org/std/primitive.slice.html#method.binary_search_by) ((& T) -> [Ordering](https://doc.rust-lang.org/std/cmp/enum.Ordering.html))  -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html), [usize](https://doc.rust-lang.org/std/primitive.usize.html)>
fn  [binary_search_by_key](https://doc.rust-lang.org/std/primitive.slice.html#method.binary_search_by_key) (& B, (& T) -> B) -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html), [usize](https://doc.rust-lang.org/std/primitive.usize.html)> where  B: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
## Getting and iterating
fn  [first](https://doc.rust-lang.org/std/primitive.slice.html#method.first) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<& T>
fn  [last](https://doc.rust-lang.org/std/primitive.slice.html#method.last)  () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<& T>
fn  [get](https://doc.rust-lang.org/std/primitive.slice.html#method.get) ([usize](https://doc.rust-lang.org/std/primitive.usize.html) | [RangeBounds](https://doc.rust-lang.org/std/ops/trait.RangeBounds.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<& T>
fn  [iter](https://doc.rust-lang.org/std/primitive.slice.html#method.iter) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & T>
## Length
fn  [len](https://doc.rust-lang.org/std/primitive.slice.html#method.len) () -> [usize](https://doc.rust-lang.org/std/primitive.usize.html)
fn  [is_empty](https://doc.rust-lang.org/std/primitive.slice.html#method.is_empty) () -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
[&mut [T]](https://doc.rust-lang.org/std/primitive.slice.html)
## Splitting to iterator
fn  [split_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.split_mut)  ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  [T]>
fn  [rsplit_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.rsplit_mut) ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  [T]>
fn  [splitn_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.splitn_mut)  ([usize](https://doc.rust-lang.org/std/primitive.usize.html), (& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  [T]>
fn  [rsplitn_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.rsplitn_mut) ([usize](https://doc.rust-lang.org/std/primitive.usize.html), (& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  [T]>
## Splitting at position
fn  [split_at_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.split_at_mut) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> (& mut  [T], & mut  [T])
fn  [split_first_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.split_first_mut) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<(& mut  T, & mut  [T])>
fn  [split_last_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.split_last_mut)  () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<(& mut  T, & mut  [T])>
## Chunks
fn  [chunks_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.chunks_mut)        ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  [T]>
fn  [chunks_exact_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.chunks_exact_mut)  ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  [T]>
fn  [rchunks_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.rchunks_mut)       ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  [T]>
fn  [rchunks_exact_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.rchunks_exact_mut) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  [T]>
## Sorting
fn  [sort](https://doc.rust-lang.org/std/primitive.slice.html#method.sort) () where  T: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
fn  [sort_by](https://doc.rust-lang.org/std/primitive.slice.html#method.sort_by) ((& T, & T) -> [Ordering](https://doc.rust-lang.org/std/cmp/enum.Ordering.html))
fn  [sort_by_key](https://doc.rust-lang.org/std/primitive.slice.html#method.sort_by_key) ((& T) -> K) where  K: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
fn  [sort_by_cached_key](https://doc.rust-lang.org/std/primitive.slice.html#method.sort_by_cached_key) ((& T) -> K) where  K: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
fn  [sort_unstable](https://doc.rust-lang.org/std/primitive.slice.html#method.sort_unstable) () where  T: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
fn  [sort_unstable_by](https://doc.rust-lang.org/std/primitive.slice.html#method.sort_unstable_by) ((& T, & T) -> [Ordering](https://doc.rust-lang.org/std/cmp/enum.Ordering.html))
fn  [sort_unstable_by_key](https://doc.rust-lang.org/std/primitive.slice.html#method.sort_unstable_by_key) ((& T) -> K) where  K: [Ord](https://doc.rust-lang.org/std/cmp/trait.Ord.html)
## Rearranging
fn  [swap](https://doc.rust-lang.org/std/primitive.slice.html#method.swap) ([usize](https://doc.rust-lang.org/std/primitive.usize.html), [usize](https://doc.rust-lang.org/std/primitive.usize.html))
fn  [reverse](https://doc.rust-lang.org/std/primitive.slice.html#method.reverse) ()
fn  [rotate_left](https://doc.rust-lang.org/std/primitive.slice.html#method.rotate_left) ([usize](https://doc.rust-lang.org/std/primitive.usize.html))
fn  [rotate_right](https://doc.rust-lang.org/std/primitive.slice.html#method.rotate_right) ([usize](https://doc.rust-lang.org/std/primitive.usize.html))
## Overriding
fn  [swap_with_slice](https://doc.rust-lang.org/std/primitive.slice.html#method.swap_with_slice)  (& mut  [T])
fn  [copy_from_slice](https://doc.rust-lang.org/std/primitive.slice.html#method.copy_from_slice)  (& [T]) where  T: [Copy](https://doc.rust-lang.org/std/marker/trait.Copy.html)
fn  [clone_from_slice](https://doc.rust-lang.org/std/primitive.slice.html#method.clone_from_slice) (& [T]) where  T: [Clone](https://doc.rust-lang.org/std/clone/trait.Clone.html)
## Getting and iterating
fn  [first_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.first_mut) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<& mut  T>
fn  [last_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.last_mut)  () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<& mut  T>
fn  [get_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.get_mut) ([usize](https://doc.rust-lang.org/std/primitive.usize.html) | [RangeBounds](https://doc.rust-lang.org/std/ops/trait.RangeBounds.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<& mut  T>
fn  [iter_mut](https://doc.rust-lang.org/std/primitive.slice.html#method.iter_mut) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & mut  T>
[&mut Vec<T>](https://doc.rust-lang.org/std/vec/struct.Vec.html)
## Adding and removing single item
fn  [push](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.push) (T)
fn  [pop](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.pop) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<T>
fn  [insert](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.insert) ([usize](https://doc.rust-lang.org/std/primitive.usize.html), T)
fn  [remove](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.remove) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> T
fn  [swap_remove](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.swap_remove) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> T
## Extending
fn  [append](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.append) (& mut  Vec<T>)
fn  [extend](https://doc.rust-lang.org/std/vec/struct.Vec.html#impl-Extend%3CT%3E) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>)
fn  [extend](https://doc.rust-lang.org/std/vec/struct.Vec.html#impl-Extend%3C%26%27a%20T%3E) ([IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = & T>) where  T: [Copy](https://doc.rust-lang.org/std/marker/trait.Copy.html)
fn  [extend_from_slice](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.extend_from_slice) (& [T]) where  T: [Clone](https://doc.rust-lang.org/std/clone/trait.Clone.html)
## Resizing
fn  [truncate](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.truncate) ([usize](https://doc.rust-lang.org/std/primitive.usize.html))
fn  [resize](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.resize) ([usize](https://doc.rust-lang.org/std/primitive.usize.html), T) where  T: [Clone](https://doc.rust-lang.org/std/clone/trait.Clone.html)
fn  [resize_with](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.resize_with) ([usize](https://doc.rust-lang.org/std/primitive.usize.html), () -> T)
## Clearing
fn  [clear](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.clear) ()
fn  [retain](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.retain) ((& T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html))
## Removing or replacing range into iterator
fn  [drain](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.drain)  ([RangeBounds](https://doc.rust-lang.org/std/ops/trait.RangeBounds.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<T>
fn  [splice](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.splice) ([RangeBounds](https://doc.rust-lang.org/std/ops/trait.RangeBounds.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>, [IntoIterator](https://doc.rust-lang.org/std/iter/trait.IntoIterator.html)<Item  = T>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<T>
## Deduplicating
fn  [dedup](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.dedup) () where  T: [PartialEq](https://doc.rust-lang.org/std/cmp/trait.PartialEq.html)
fn  [dedup_by](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.dedup_by) ((& mut  T, & mut  T) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html))
fn  [dedup_by_key](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.dedup_by_key) ((& mut  T) -> K) where  K: [PartialEq](https://doc.rust-lang.org/std/cmp/trait.PartialEq.html)
## Splitting off
fn  [split_off](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.split_off) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> Vec<T>
## Capacity manipulation
fn  [reserve](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.reserve) ([usize](https://doc.rust-lang.org/std/primitive.usize.html))
fn  [reserve_exact](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.reserve_exact) ([usize](https://doc.rust-lang.org/std/primitive.usize.html))
fn  [shrink_to_fit](https://doc.rust-lang.org/std/vec/struct.Vec.html#method.shrink_to_fit) ()
[&[u8]](https://doc.rust-lang.org/std/primitive.slice.html)
## ASCII
fn  [is_ascii](https://doc.rust-lang.org/std/primitive.slice.html#method.is_ascii) () -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
fn  [eq_ignore_ascii_case](https://doc.rust-lang.org/std/primitive.slice.html#method.eq_ignore_ascii_case) (& [[u8](https://doc.rust-lang.org/std/primitive.u8.html)]) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
fn  [to_ascii_uppercase](https://doc.rust-lang.org/std/primitive.slice.html#method.to_ascii_uppercase) () -> Vec<[u8](https://doc.rust-lang.org/std/primitive.u8.html)>
fn  [to_ascii_lowercase](https://doc.rust-lang.org/std/primitive.slice.html#method.to_ascii_lowercase) () -> Vec<[u8](https://doc.rust-lang.org/std/primitive.u8.html)>
[&mut [u8]](https://doc.rust-lang.org/std/primitive.slice.html)
## ASCII
fn  [make_ascii_uppercase](https://doc.rust-lang.org/std/primitive.slice.html#method.make_ascii_uppercase) ()
fn  [make_ascii_lowercase](https://doc.rust-lang.org/std/primitive.slice.html#method.make_ascii_lowercase) ()
[&str](https://doc.rust-lang.org/std/primitive.str.html)
## Chars
fn  [chars](https://doc.rust-lang.org/std/primitive.str.html#method.chars) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = [char](https://doc.rust-lang.org/std/primitive.char.html)>
fn  [char_indices](https://doc.rust-lang.org/std/primitive.str.html#method.char_indices) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = ([usize](https://doc.rust-lang.org/std/primitive.usize.html), [char](https://doc.rust-lang.org/std/primitive.char.html))>
fn  [is_char_boundary](https://doc.rust-lang.org/std/primitive.str.html#method.is_char_boundary) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
## Bytes
fn  [bytes](https://doc.rust-lang.org/std/primitive.str.html#method.bytes) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = [u8](https://doc.rust-lang.org/std/primitive.u8.html)>
fn  [as_bytes](https://doc.rust-lang.org/std/primitive.str.html#method.as_bytes) () -> & [[u8](https://doc.rust-lang.org/std/primitive.u8.html)]
## Splitting to two parts
fn  [split_at](https://doc.rust-lang.org/std/primitive.str.html#method.split_at) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> (& [str](https://doc.rust-lang.org/std/primitive.str.html), & [str](https://doc.rust-lang.org/std/primitive.str.html))
## Splitting to iterator
fn  [lines](https://doc.rust-lang.org/std/primitive.str.html#method.lines) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [split_whitespace](https://doc.rust-lang.org/std/primitive.str.html#method.split_whitespace) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [split_ascii_whitespace](https://doc.rust-lang.org/std/primitive.str.html#method.split_ascii_whitespace) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [split](https://doc.rust-lang.org/std/primitive.str.html#method.split)  ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [rsplit](https://doc.rust-lang.org/std/primitive.str.html#method.rsplit) ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [splitn](https://doc.rust-lang.org/std/primitive.str.html#method.splitn)  ([usize](https://doc.rust-lang.org/std/primitive.usize.html), [char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [rsplitn](https://doc.rust-lang.org/std/primitive.str.html#method.rsplitn) ([usize](https://doc.rust-lang.org/std/primitive.usize.html), [char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [split_terminator](https://doc.rust-lang.org/std/primitive.str.html#method.split_terminator)  ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [rsplit_terminator](https://doc.rust-lang.org/std/primitive.str.html#method.rsplit_terminator) ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
## Trimming
fn  [trim](https://doc.rust-lang.org/std/primitive.str.html#method.trim)       () -> & [str](https://doc.rust-lang.org/std/primitive.str.html)
fn  [trim_start](https://doc.rust-lang.org/std/primitive.str.html#method.trim_start) () -> & [str](https://doc.rust-lang.org/std/primitive.str.html)
fn  [trim_end](https://doc.rust-lang.org/std/primitive.str.html#method.trim_end)   () -> & [str](https://doc.rust-lang.org/std/primitive.str.html)
fn  [trim_matches](https://doc.rust-lang.org/std/primitive.str.html#method.trim_matches)       ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> & [str](https://doc.rust-lang.org/std/primitive.str.html)
fn  [trim_start_matches](https://doc.rust-lang.org/std/primitive.str.html#method.trim_start_matches) ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> & [str](https://doc.rust-lang.org/std/primitive.str.html)
fn  [trim_end_matches](https://doc.rust-lang.org/std/primitive.str.html#method.trim_end_matches)   ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> & [str](https://doc.rust-lang.org/std/primitive.str.html)
## Matching and finding
fn  [contains](https://doc.rust-lang.org/std/primitive.str.html#method.contains)    ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
fn  [starts_with](https://doc.rust-lang.org/std/primitive.str.html#method.starts_with) ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
fn  [ends_with](https://doc.rust-lang.org/std/primitive.str.html#method.ends_with)   ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
fn  [find](https://doc.rust-lang.org/std/primitive.str.html#method.find)  ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>
fn  [rfind](https://doc.rust-lang.org/std/primitive.str.html#method.rfind) ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>
fn  [matches](https://doc.rust-lang.org/std/primitive.str.html#method.matches)  ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [rmatches](https://doc.rust-lang.org/std/primitive.str.html#method.rmatches) ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = & [str](https://doc.rust-lang.org/std/primitive.str.html)>
fn  [match_indices](https://doc.rust-lang.org/std/primitive.str.html#method.match_indices)  ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = ([usize](https://doc.rust-lang.org/std/primitive.usize.html), & [str](https://doc.rust-lang.org/std/primitive.str.html))>
fn  [rmatch_indices](https://doc.rust-lang.org/std/primitive.str.html#method.rmatch_indices) ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = ([usize](https://doc.rust-lang.org/std/primitive.usize.html), & [str](https://doc.rust-lang.org/std/primitive.str.html))>
## Case
fn  [to_uppercase](https://doc.rust-lang.org/std/primitive.str.html#method.to_uppercase) () -> [String](https://doc.rust-lang.org/std/string/trait.String.html)
fn  [to_lowercase](https://doc.rust-lang.org/std/primitive.str.html#method.to_lowercase) () -> [String](https://doc.rust-lang.org/std/string/trait.String.html)
fn  [to_ascii_uppercase](https://doc.rust-lang.org/std/primitive.str.html#method.to_ascii_uppercase) () -> [String](https://doc.rust-lang.org/std/string/trait.String.html)
fn  [to_ascii_lowercase](https://doc.rust-lang.org/std/primitive.str.html#method.to_ascii_lowercase) () -> [String](https://doc.rust-lang.org/std/string/trait.String.html)
fn  [eq_ignore_ascii_case](https://doc.rust-lang.org/std/primitive.str.html#method.eq_ignore_ascii_case) (& [str](https://doc.rust-lang.org/std/primitive.str.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
## Replacing
fn  [replace](https://doc.rust-lang.org/std/primitive.str.html#method.replace)  ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html), & [str](https://doc.rust-lang.org/std/primitive.str.html)) -> [String](https://doc.rust-lang.org/std/string/trait.String.html)
fn  [replacen](https://doc.rust-lang.org/std/primitive.str.html#method.replacen) ([char](https://doc.rust-lang.org/std/primitive.char.html) | & [str](https://doc.rust-lang.org/std/primitive.str.html) | & [[char](https://doc.rust-lang.org/std/primitive.char.html)] | ([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html), & [str](https://doc.rust-lang.org/std/primitive.str.html), [usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [String](https://doc.rust-lang.org/std/string/trait.String.html)
## Length
fn  [len](https://doc.rust-lang.org/std/primitive.str.html#method.len) () -> [usize](https://doc.rust-lang.org/std/primitive.usize.html)
fn  [is_empty](https://doc.rust-lang.org/std/primitive.str.html#method.is_empty) () -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
## Misc.
fn  [is_ascii](https://doc.rust-lang.org/std/primitive.str.html#method.is_ascii) () -> [bool](https://doc.rust-lang.org/std/primitive.bool.html)
fn  [repeat](https://doc.rust-lang.org/std/primitive.str.html#method.repeat) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [String](https://doc.rust-lang.org/std/string/trait.String.html)
fn  [encode_utf16](https://doc.rust-lang.org/std/primitive.str.html#method.encode_utf16) () -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = [u16](https://doc.rust-lang.org/std/primitive.u16.html)>
fn  [parse](https://doc.rust-lang.org/std/primitive.str.html#method.parse) () -> [Result](https://doc.rust-lang.org/std/result/enum.Result.html)<F, E> where  F: [FromStr](https://doc.rust-lang.org/std/str/trait.FromStr.html)
[&mut str](https://doc.rust-lang.org/std/primitive.str.html)
## Splitting to two parts
fn  [split_at_mut](https://doc.rust-lang.org/std/primitive.str.html#method.split_at_mut) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> (& mut  [str](https://doc.rust-lang.org/std/primitive.str.html), & mut  [str](https://doc.rust-lang.org/std/primitive.str.html))
## Case conversion
fn  [make_ascii_uppercase](https://doc.rust-lang.org/std/primitive.str.html#method.make_ascii_uppercase) ()
fn  [make_ascii_lowercase](https://doc.rust-lang.org/std/primitive.str.html#method.make_ascii_lowercase) ()
[&mut String](https://doc.rust-lang.org/std/string/struct.String.html)
## Inserting and appending string
fn  [push_str](https://doc.rust-lang.org/std/string/struct.String.html#method.push_str) (& [str](https://doc.rust-lang.org/std/primitive.str.html))
fn  [insert_str](https://doc.rust-lang.org/std/string/struct.String.html#method.insert_str) ([usize](https://doc.rust-lang.org/std/primitive.usize.html), & [str](https://doc.rust-lang.org/std/primitive.str.html))
## Adding and removing char
fn  [push](https://doc.rust-lang.org/std/string/struct.String.html#method.push) ([char](https://doc.rust-lang.org/std/primitive.char.html))
fn  [pop](https://doc.rust-lang.org/std/string/struct.String.html#method.pop) () -> [Option](https://doc.rust-lang.org/std/option/enum.Option.html)<[char](https://doc.rust-lang.org/std/primitive.char.html)>
fn  [insert](https://doc.rust-lang.org/std/string/struct.String.html#method.insert) ([usize](https://doc.rust-lang.org/std/primitive.usize.html), [char](https://doc.rust-lang.org/std/primitive.char.html))
fn  [remove](https://doc.rust-lang.org/std/string/struct.String.html#method.remove) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [char](https://doc.rust-lang.org/std/primitive.char.html)
## Clearing
fn  [clear](https://doc.rust-lang.org/std/string/struct.String.html#method.clear) ()
fn  [truncate](https://doc.rust-lang.org/std/string/struct.String.html#method.truncate) ([usize](https://doc.rust-lang.org/std/primitive.usize.html))
fn  [retain](https://doc.rust-lang.org/std/string/struct.String.html#method.retain) (([char](https://doc.rust-lang.org/std/primitive.char.html)) -> [bool](https://doc.rust-lang.org/std/primitive.bool.html))
## Capacity manipulation
fn  [reserve](https://doc.rust-lang.org/std/string/struct.String.html#method.reserve) ([usize](https://doc.rust-lang.org/std/primitive.usize.html))
fn  [reserve_exact](https://doc.rust-lang.org/std/string/struct.String.html#method.reserve_exact) ([usize](https://doc.rust-lang.org/std/primitive.usize.html))
fn  [shrink_to_fit](https://doc.rust-lang.org/std/string/struct.String.html#method.shrink_to_fit) ()
## Misc.
fn  [split_off](https://doc.rust-lang.org/std/string/struct.String.html#method.split_off) ([usize](https://doc.rust-lang.org/std/primitive.usize.html)) -> [String](https://doc.rust-lang.org/std/string/trait.String.html)
fn  [replace_range](https://doc.rust-lang.org/std/string/struct.String.html#method.replace_range) ([RangeBounds](https://doc.rust-lang.org/std/ops/trait.RangeBounds.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>, & [str](https://doc.rust-lang.org/std/primitive.str.html))
fn  [drain](https://doc.rust-lang.org/std/string/struct.String.html#method.drain) ([RangeBounds](https://doc.rust-lang.org/std/ops/trait.RangeBounds.html)<[usize](https://doc.rust-lang.org/std/primitive.usize.html)>) -> [Iterator](https://doc.rust-lang.org/std/iter/trait.Iterator.html)<Item  = [char](https://doc.rust-lang.org/std/primitive.char.html)>
